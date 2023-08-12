<script setup>
import {ref} from "vue";

const skillView = ref(['HTML/CSS', 'JavaScript', 'vue.js', 'nuxt3'])
const frontEnd = ['HTML/CSS', 'JavaScript', 'vue.js', 'nuxt3']
const backEnd = ['Java', 'Spring Boot']
const database = ['SQL']
function viewSkill (skillType) {
  if (skillType === 'front') {
    skillView.value = frontEnd
  } else if (skillType === 'back') {
    skillView.value = backEnd
  } else {
    skillView.value = database
  }
}
</script>

<template>
  <div>
    <link href="https://fonts.cdnfonts.com/css/atari" rel="stylesheet">
    <div class="sectionTitle" style="font-family: 'Atari', sans-serif; text-shadow: 0 0 20px limegreen, 0 0 30px darkgreen">
      TECHNICAL SKILLS
    </div>
    <div class="skillList">
      <button @click="viewSkill('front')">front-end</button>
      <button @click="viewSkill('back')">back-end</button>
      <button @click="viewSkill('data')">database</button>
    </div>
    <ul class="skills">
      <li v-for="skill in skillView">
        {{ skill }}
      </li>
    </ul>
  </div>
</template>

<style scoped>
.skills {
  display: flex;
  justify-content: center;
  height: 100px;
  font-size: 20px; /* 14px */
  line-height: 100px; /* 20px */
  margin-top: 40px;
}
.skills li {
  margin-inline: 40px;
  color: white;
  font-family: 'Atari', sans-serif;
}
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
  font-family: Atari, sans-serif;
  margin-inline: 140px;
}
.skillList button:hover{
  text-shadow: 0 0 30px green, 0 0 20px darkgreen;
}
.skillList button:focus{
  border: 7px solid white;
  padding-inline: 30px;
}
</style>
