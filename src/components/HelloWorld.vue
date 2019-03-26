<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p v-html="head"></p>
    <div v-for="menu in menus" :key="menu.headline">
      <h3>{{ menu.headline }}</h3>
      <ul>
        <li v-for="link in menu.links" :key="link.text"><a :href="link.href">{{ link.text }}</a></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: {
      type: String,
      default: 'HelloWorld'
    }
  },
  data: function(){
    return{
      head: 'For a guide and recipes on how to configure / customize this project,<br>check out the <a style="color: #42b983;" href="https://cli.vuejs.org" target="_blank">Стандартный инструментарий для разработки на Vue.js</a>',
      menus: [
        {
          headline: 'Installed CLI Plugins',
          links: [
            { text:'babel', href:'https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel' },
            { text:'eslint', href:'https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint' },
          ]
        },
        {
          headline: 'Essential Links',
          links: [
            { text:'Core Docs', href:'https://vuejs.org' },
            { text:'Forum', href:'https://forum.vuejs.org' },
            { text:'Community Chat', href:'https://chat.vuejs.org' },
            { text:'Twitter', href:'https://twitter.com/vuejs' },
            { text:'News', href:'https://news.vuejs.org' }
          ]
        },
        {
          headline: 'Ecosystem',
          links: [
            { text:'vue-router', href:'https://router.vuejs.org' },
            { text:'vuex', href:'https://vuex.vuejs.org' },
            { text:'vue-devtools', href:'https://github.com/vuejs/vue-devtools#vue-devtools' },
            { text:'vue-loader', href:'https://vue-loader.vuejs.org' },
            { text:'awesome-vue', href:'https://github.com/vuejs/awesome-vue' },
          ]
        }
      ]
    }
  }
};

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
