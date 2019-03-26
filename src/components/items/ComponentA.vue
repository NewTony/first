<template>
<li>{{ todo.text }}</li>
</template>

<script>
export default {
name: 'component-a',
data: function() {
  return {

    }
  },
props: {
  msg:
  {
    type: String,
    default: 'Компонент А'
  },
  todo: {}
},
components:
{
}
}
</script>

<style scoped>
  li {
    display: block;
    margin: 0 10px;
  }
</style>
