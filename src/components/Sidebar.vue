<template>
  <div>
    <img id="headshot" alt="Headshot" src="../assets/headshot.png" />
    <h1>Frank Mazzarella</h1>
    <h3>Scranton, PA</h3>
    <ul>
      <li>mazzarella.frank@gmail.com</li>
      <li>570.351.1791</li>
      <li>frankmazz.com</li>
      <li>github.com/frankmazzarella</li>
      <li>linkedin.com/in/frankmazzarella</li>
    </ul>
    <button>Download</button>
    <button>Drop me a line</button>
    <h3>Education</h3>
    <ul>
      <li>Misericordia University</li>
      <li>Computer Science BS</li>
      <li>Graduated December 2015</li>
    </ul>
    <button>Fork me on GitHub</button>
  </div>
</template>

<script>
export default {
  name: 'Sidebar',
};
</script>

<style scoped>
#headshot {
  margin: 50px 10px 0;
  width: 250px;
  height: 250px;
  border-radius: 35%;
}

li {
  text-align: left;
}
</style>
