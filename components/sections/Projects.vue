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
  <div style="">
    <div class="anchor"></div>
    <div class="sectionTitle" style="font-family: 'Atari', sans-serif; text-shadow: 0 0 20px limegreen, 0 0 30px darkgreen">
      TECHNICAL PROJECTS
    </div>
  </div>
</template>

<style scoped>

</style>
