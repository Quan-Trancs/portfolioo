<script setup>
</script>

<template>
  <div>
    <div class="sectionTitle">TECHNICAL SKILLS</div>
    <div class="skillList">
      <button>front-end</button>
      <button>back-end</button>
      <button>database</button>
    </div>
  </div>
</template>

<style scoped>
.skillList {
  display: flex;
  justify-content: center;
  height: 100px;
  font-size: 0.875rem; /* 14px */
  line-height: 1.25rem; /* 20px */
}
.skillList button {
  background: none;
  border: none;
  color: white;
  font-size: 32px;
  margin-inline: 140px;
}
.skillList button:hover{
  border: 10px solid green;
}
.skillList button:focus{
  border: 10px solid white;
}
</style>
