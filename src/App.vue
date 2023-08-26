<template>
<Portfolio/>
</template>

<script>
import Portfolio from './components/Portfolio.vue'

export default {
  name: 'App',
  components: {
    Portfolio
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}
*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
html,body{
    margin: 0;
    padding: 0;
    height: 500vh;
    width:100% ;
}
</style>
