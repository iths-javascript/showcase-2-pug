<template lang="pug">
#app
  header
    span.logo.large.semi-round
    nav
      router-link(to="/about")
  main
    h1 Hello World
    ul
      li(
        v-for="item in list"
        :key="item"
      ) {{item}}
</template>

<script>

export default {
  name: 'App',
  data(){return {
    list: ['Äpple', 'Banan', 'Grillkorv']
  }}
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
