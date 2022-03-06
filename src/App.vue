<template>
  <Headerbar username="Eric"/>
  <Sidebar v-bind:active="false"/>
</template>

<script>
import Pagebody from './components/Pagebody.vue'
import Headerbar from './components/Headerbar.vue'
import Sidebar from './components/Sidebar.vue'
import Homepage from './components/pagebody/Homepage.vue'

export default {
  name: 'App',
  components: {
    Headerbar,
    Homepage,
    Sidebar
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
