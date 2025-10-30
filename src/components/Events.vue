<template>
      <!-- using event Access the event object -->
      <input @click="onInput" placeholder="Type something" />
</template>

<script setup>
   function onInput(event) {
    console.log('Input value value:', event.target.value)
   }
</script>