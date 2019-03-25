<template>
<div id="phones">
  <p>{{msg}}</p>
</div>
</template>

<script>
export default {
name: 'ComponentA',
data: function() {
  return {

    }
  },
props: {
  msg: {
    type: String,
    default: 'Компонент А'
  }
},
components: {
}
}
</script>
