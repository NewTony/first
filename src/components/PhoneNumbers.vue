<template>
  <div id="phones">
    <h3>{{ msg }}</h3>
    <ol><component-a v-for="item in groceryList" v-bind:todo="item" v-bind:key="item.id"></component-a></ol>
  </div>
</template>

<script>

import ComponentA from './items/ComponentA.vue'

export default {
name: 'PhoneNumbers',
data: function() {
  return {
    groceryList: [
        { id: 0, text: 'Овощи' },
        { id: 1, text: 'Сыр' },
        { id: 2, text: 'Что там ещё люди едят?' }
      ]
    }
  },
props: {
  msg: {
    type: String,
    default: 'Телефонный справочник'
  }
},
components: {
  'component-a': ComponentA
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
