<template>
  <div id="phones">
    <h3>{{ msg }}</h3>
    <component-a/>
  </div>
</template>

<script>

import ComponentA from './items/ComponentA.vue'

export default {
name: 'PhoneNumbers',
data: function() {
  return {

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
