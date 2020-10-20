<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <h1>Belajar Vue Hook</h1>
  <Navbar/>
  <Blogs/>
</template>

<script>
import Navbar from './components/Navbar'
import Blogs from './components/Blogs'

export default {
  name: 'App',
  components: {
    Navbar,
    Blogs
  },
  data() {
    return {
      title : 'Yuk Main Vue js'
    }
  },
  methods : {

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
