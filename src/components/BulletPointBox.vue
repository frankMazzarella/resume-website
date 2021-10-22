<template>
  <div id="bullet-point-box">
    <p>{{ title }}</p>
    <ul>
      <li v-for="(bulletpoint, index) in bulletpoints" :key="index">{{ bulletpoint }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'BulletPointBox',
  props: ['title', 'bulletpoints'],
};
</script>

<style scoped>
#bullet-point-box {
  margin: 10px;
  background-color: #ccc;
  border-radius: 10px;
}
</style>
