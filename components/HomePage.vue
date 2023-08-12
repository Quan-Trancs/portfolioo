<script setup>

</script>

<template>
  <div class="bg-image">
    <TheHeader/>
    <TheBody/>
    <TheFooter class="footer"/>
  </div>
</template>

<style scoped>
.bg-image {
  background-image: url('static/bg.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
}
.footer {
  margin-top: auto;
}
</style>
