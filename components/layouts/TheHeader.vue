<script setup>
</script>

<template>
  <div class="header h-[200px] bg-blue px-2 py-2.5 py-5 text-white sm:px-4">
    <div class="container mx-auto flex flex-wrap items-center">
      <ul class="navigation">
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
}
.container {
  height: 120px;
  background: white;
}
.navigation {
  margin-top: 40px;
  display: flex;
  list-style-type: none;
  font-size: 40px;
}
.navigation li {
  margin-right: 30px;
  text-decoration: none;
}
</style>
