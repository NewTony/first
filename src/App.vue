<template>
  <div id="app">
    <div id="header">
      <div class="logo">
        <img style="width: 50px;" alt="Logo" src="./assets/logo.png">
      </div>
      <div class="title">
        Title
      </div>
    </div>
    <div id="body">
      <HelloWorld/>
      <PhoneNumbers/>
    </div>
    <div id="footer"></div>
  </div>
</template>

<script>

import HelloWorld from './components/HelloWorld.vue'
import PhoneNumbers from './components/PhoneNumbers.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    PhoneNumbers
  }
}
</script>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  /* margin-top: 60px; */
}

#header {
  height: 100px;
  display: block;
}

#body {
  display: block;
}

#footer {
  height: 100px;
  display: block;
}

.title {
  display: inline-block;
}

.content {

}

.logo {
  display: inline-block;
}

</style>
