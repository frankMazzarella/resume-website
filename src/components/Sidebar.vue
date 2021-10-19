<template>
  <div id="sidebar">
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
/* @media (max-width: 800px) { */
/* TODO: should this be in media query?? idk */
  #sidebar {
    width: 400px;
    margin: 0 auto;
  }
/* } */

#headshot {
  margin-top: 50px;
  width: 250px;
  height: 250px;
  border-radius: 35%;
}

h1, h3 {
  margin: 0;
}

ul {
  margin-top: 10px;
  padding-left: 80px;
  text-align: left;
}

button {
  margin-bottom: 10px;
}
</style>
