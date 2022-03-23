<template>
  <div id="app">
    <HelloWorld/>
    <BlackLine/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import BlackLine from './components/BlackLine.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    BlackLine
  }
}
</script>

<style lang="scss">
  *{
    margin: 0;
    box-sizing: 0;
  }

  #app{
    background-color: black;
    padding-top: 1rem;
  }
</style>
