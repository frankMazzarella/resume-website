<template>
  <div id="app">
    <Sidebar id="sidebar" />
    <div id="main-content">
      <p v-for="index in 100" :key="index">main content</p>
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue';

export default {
  name: 'App',
  components: {
    Sidebar,
  },
};
</script>

<style scoped>
#app {
  display: flex;
  max-width: 800px;
  margin: 0 auto;
}

@media (min-width: 800px) {
  #sidebar {
    flex-grow: 1;
    height: 100vh;
    overflow-y: scroll;
    border-right: dashed #808080;
  }

  #main-content {
    flex-grow: 4;
    height: 100vh;
    overflow-y: scroll;
  }
}

@media (max-width: 800px) {
  #app {
    flex-direction: column;
  }
}
</style>
