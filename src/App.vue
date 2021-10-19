<template>
  <div id="container">
    <!-- <div id="app">
      <img alt="Vue logo" src="./assets/logo.png">
      <HelloWorld msg="Welcome to Your Vue.js App"/>
    </div> -->

    <div id="sidebar">
      sidebar
    </div>
    <div id="main-content">
      main content
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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#container {
  display: flex;
  max-width: 1200px;
  margin: 0 auto;
}

#sidebar {
  flex-grow: 1;
  border: solid;
  border-width: 4px;
  border-color: red;
}

#main-content {
  flex-grow: 4;
  border: solid;
  border-width: 4px;
  border-color: red;
}

@media (max-width: 1200px) {
  #container {
    flex-direction: column;
  }
}
</style>
