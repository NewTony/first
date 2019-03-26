<template>
<div id="phones">
  <p>{{msg}}</p>
</div>
</template>

<script>
export default {
name: 'component-b',
data: function() {
  return {

    }
  },
props: {
  msg: {
    type: String,
    default: 'Компонент B'
  }
},
components: {
}
}
</script>
