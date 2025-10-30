<template>
  <!-- <div class="ms-[700px] p-8 text-gray-600  mt-[100px] w-[400px] rounded-lg shadow-2xl">
    <h1 class="text-center text-lg font-bold">Welcome to My Vue App</h1>
    <p class="text-center text-gray-500">Start building your component here!</p>
    <HelloWorld />
  </div> -->

  <div>
    <!-- <Interpolation /> -->
     <!-- <Counter /> -->
     <Directives />
  </div>
</template>

<script setup>
     import Counter from './components/Counter.vue';
     import Directives from './components/Directives.vue';
     import HelloWorld from './components/HelloWorld.vue';
     import Interpolation from './components/Interpolation.vue';
</script>
