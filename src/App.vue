<template>
  <div id="app">
    <HelloWorld/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
    body {
        padding: 0;
        margin: 0;
        font-family: 'Karla', sans-serif;
    }
</style>
