<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <AgeInput />
</template>

<script>
import AgeInput from './components/AgeInput.vue'

export default {
  name: 'App',
  components: {
    AgeInput
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
