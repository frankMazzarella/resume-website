<template>
  <div id="container">
    <!-- <div id="app">
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div> -->

    <div id="sidebar">
      <p v-for="index in 10" :key="index">sidebar</p>
    </div>
    <div id="main-content">
      <p v-for="index in 100" :key="index">main content</p>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
  }
}
</script>

<style>
#container {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
}

@media (min-width: 1200px) {
  #sidebar {
    flex-grow: 1;
    height: 100vh;
    overflow-y: scroll;
  }

  #main-content {
    flex-grow: 4;
    height: 100vh;
    overflow-y: scroll;
  }
}

@media (max-width: 1200px) {
  #container {
    flex-direction: column;
  }
}
</style>
