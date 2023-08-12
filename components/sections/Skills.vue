<script setup>
import {ref} from "vue";

const skillView = ref(['HTML/CSS', 'JavaScript', 'vue.js', 'nuxt3'])
const skillType = ref('front')
const frontEnd = ['HTML/CSS', 'JavaScript', 'vue.js', 'nuxt3']
const backEnd = ['Java', 'Spring Boot']
const database = ['SQL']
function skillTypeCheck (chosenSkillType) {
  return (skillType.value === chosenSkillType)
}
function viewSkill (chosenSkillType) {
  skillType.value = chosenSkillType
  if (chosenSkillType === 'front') {
    skillView.value = frontEnd
  } else if (chosenSkillType === 'back') {
    skillView.value = backEnd
  } else {
    skillView.value = database
  }
}
</script>

<template>
  <div style="margin-top: 200px">
    <div class="sectionTitle" style="font-family: 'Atari', sans-serif; text-shadow: 0 0 20px limegreen, 0 0 30px darkgreen">
      TECHNICAL SKILLS
    </div>
    <div class="skillList">
      <button v-if="skillTypeCheck('front')" style="text-shadow: 0 0 30px green, 0 0 20px darkgreen;" @click="viewSkill('front')">front-end</button>
      <button v-if="!skillTypeCheck('front')" @click="viewSkill('front')">front-end</button>
      <button v-if="skillTypeCheck('back')" style="text-shadow: 0 0 30px green, 0 0 20px darkgreen;" @click="viewSkill('back')">back-end</button>
      <button v-if="!skillTypeCheck('back')" @click="viewSkill('back')">back-end</button>
      <button v-if="skillTypeCheck('data')" style="text-shadow: 0 0 30px green, 0 0 20px darkgreen;" @click="viewSkill('data')">database</button>
      <button v-if="!skillTypeCheck('data')" @click="viewSkill('data')">database</button>
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
  list-style-type: none;
  height: 100px;
  font-size: 30px; /* 14px */
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
  text-shadow: 0 0 30px green, 0 0 20px darkgreen;

}
</style>
