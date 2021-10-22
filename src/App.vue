<template>
  <div id="app">
    <Sidebar id="sidebar" />
    <div id="main-content">
      <Bio />
      <bullet-point-box :title="skills.description" :bulletpoints="skills.list" />
      <bullet-point-box :title="jobs.description" :bulletpoints="jobs.list" />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/Sidebar.vue';
import Bio from './components/Bio.vue';
import BulletPointBox from './components/BulletPointBox.vue';

export default {
  name: 'App',
  data: () => ({
    skills: {
      description: 'Skills I Provide',
      list: [
        'skill one',
        'skill two',
        'skill three',
      ],
    },
    jobs: {
      description: 'Jobs I Want',
      list: [
        'job one',
        'job two',
      ],
    },
  }),
  components: {
    Sidebar,
    Bio,
    BulletPointBox,
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
    height: 100vh;
    border-right: dashed #808080;
  }

  #main-content {
    height: 100vh;
    overflow: scroll;
  }
}

@media (max-width: 800px) {
  #app {
    flex-direction: column;
  }
}
</style>
