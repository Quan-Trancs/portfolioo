<script setup>

</script>

<template>
  <div>
    <div class="sectionTitle">ABOUT ME</div>
    <div class="commandContainer">
      <div class="flex overflow-x-scroll typewriter">
        <p class="">Hi!</p>
        <p class="">My name is Quan.</p>
        <p class="">I am a student of Computer Science at Arizona State University.</p>
        <p class="">I am deeply passionate about coding.</p>
        <p class="">I often spend my free time working on projects and learning about coding skills, or, sometime, about other techs.</p>
        <p class="">In addition to technology, i also spend time on my hobby, Gundam.</p>
      </div>
      <p class="cursor">_</p>
    </div>
  </div>
</template>

<style scoped>
.commandContainer {
  background-color: rgba(0,0,0); /* Black w/opacity/see-through */
  color: white;
  font-weight: bold;
  font-size: 18px;
  border: 5px solid #f1f1f1;
  margin: auto;
  left: 50%;
  z-index: 2;
  width: 75%;
  padding: 40px;
  font-family:monospace
}

.typewriter p {
  opacity: 0;
  overflow: hidden;
  white-space: nowrap;
  margin: 0; /* Remove default paragraph margin */
  padding: 0; /* Remove default paragraph padding */
  animation: typing 5s steps(40, end) forwards;
}
.cursor {
  color: black;
  animation: blink 1s infinite forwards;
  animation-delay: 26s;
}

@keyframes typing {
  from {
    width: 0; /* Start with zero width, making text invisible */
    opacity: 1;
  }
  to {
    width: 100%; /* Fully reveal the text */
    opacity: 1;
  }
}

@keyframes blink {
  from, to {
    color: black; /* Make the cursor invisible */
  }
  50% {
    color: white; /* Show the cursor */
  }
}

/* Add animation delays for each paragraph */
.typewriter p:nth-child(1) {
  animation-delay: 0s;
  animation-duration: 10s;
  animation-iteration-count: 0.025;
}
.typewriter p:nth-child(2) {
  animation-delay: 1s;
  animation-duration: 10s;
  animation-iteration-count: 0.2;
}
.typewriter p:nth-child(3) {
  animation-delay: 2.5s; /* 6s delay after line 1 completes */
  animation-duration: 10s;
  animation-iteration-count: 0.75;
}
.typewriter p:nth-child(4) {
  animation-delay: 8s; /* 6s delay after line 1 completes */
  animation-duration: 10s;
  animation-iteration-count: 0.3;
}
.typewriter p:nth-child(5) {
  animation-delay: 11s; /* 6s delay after line 1 completes */
  animation-duration: 10s;
  animation-iteration-count: 1;
}
.typewriter p:nth-child(6) {
  animation-delay: 20.5s; /* 6s delay after line 1 completes */
  animation-duration: 10s;
  animation-iteration-count: 0.7;
}
</style>
