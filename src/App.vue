<template>
  <img alt="logo" src="./assets/logo.png">
  <HomePage msg="Automated Business Workflows, Custom Software Integrations, and Lightning Network Node Management Services"/>
</template>

<script>
import HomePage from './components/HomePage.vue'

export default {
  name: 'App',
  components: {
    HomePage,
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 12px;
}
</style>
