<template>
  <div id="app" class="container">
    <img alt="Vue logo" src="./assets/logo_thumbnail.png" width="100px" height="100px" class="round-logo">
    <HomeScreen></HomeScreen>
  </div>
</template>

<script>
import './App.css'
import HomeScreen from './components/HomeScreen.vue'

export default {
  name: 'App',
  components: {
    HomeScreen
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
.round-logo {
  border-radius: 50%
}
</style>
