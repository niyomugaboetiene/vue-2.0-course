<template>
  <div class="app">
    <h1 class="bg-blue-500">Welcome to My Vue App</h1>
    <p>Start building your component here!</p>
    <HelloWorld />
  </div>
</template>

<script setup>
 import HelloWorld from './components/HelloWorld.vue';
</script>

<style scoped>
  .app {
    text-align: center;
    margin-top: 40px;
    font-family: 'Courier New', Courier, monospace;
  }
</style>