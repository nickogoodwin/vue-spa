<template>
<!-- 
  Nicko Goodwin
  3/10/2022

  3/10/2022
    -created Navigation
    -created hero component
    -created sectionOne component
    -created sectionTwo component
    -created Footer componenet
 -->
  <div id="app">
    <navigation></navigation>
    <main>
      <hero></hero>
      <sectionOne></sectionOne>
      <sectionTwo></sectionTwo>
      <sectionFooter></sectionFooter>
    </main>
    
    
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Hero from './components/Hero.vue'
import SectionOne from './components/SectionOne.vue'
import SectionTwo from './components/SectionTwo.vue'
import sectionFooter from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Hero,
    SectionOne,
    SectionTwo,
    sectionFooter
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}

main {
  flex: 1;
}

section {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  background-size: cover;
  background-position:center;
  background-repeat: no-repeat;
  background-attachment: fixed;
}

article {
  width: 75%;
  padding: 5em 1em;
  color: white;
  background-color: rgba(18, 18, 18,0.95);
  border-radius: 2em;
  box-shadow: 0 0 10px black;
}
</style>
