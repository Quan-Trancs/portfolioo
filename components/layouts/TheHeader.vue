<script setup>
</script>

<template>
  <div class="header bg-blue px-2 py-2.5 py-5 text-white sm:px-4 z-5">
    <div class="container mx-auto flex flex-wrap items-center">
      <ul class="navigation">
        <li><a href="#about" class="logo"><img src="static/logo/logo.jpg" alt="AQ" /></a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#projects">Projects</a></li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.header {
  position: sticky;
  top: 0;
  z-index: 10;
}
.container {
  height: 110px;
  background: white;
}
.logo {
  font-size: 70px;
  color: rebeccapurple;
}
.navigation {
  display: flex;
  list-style: none;
  justify-content: space-around;
  background-color: white;
  font-size: 40px;
  height: 100px;
}
.navigation li {
  text-decoration: none;
  margin: auto;
}
.navigation a {
  text-decoration: none;
  color: black;
  font-family: 'Atari', sans-serif;
}
</style>
