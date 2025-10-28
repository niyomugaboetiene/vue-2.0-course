<template>
   <div class="ms-[700px] mt-[100px]">
    <p class="text-center me-[900px]">{{ count }}</p>
     <button @click="increment">Increment</button>
     <button @click="reset">Reset</button>
     <button @click="decrement">Decrement</button>
   </div>     
</template>

<script setup>
    import { ref } from 'vue';

    const count = ref(0);

    function increment() {
        count.value++
    }

    function reset() {
        count.value = 0;
    }

    function decrement() {
        count.value --;
    }
</script>
