<template>
    <p>{{ count }}</p>
    <button @click="increment">+</button>
    <button @click="reset">0</button>
    <button @click="decrement">-</button>
</template>

<script setup>
    import { ref } from 'vue';

    const count = ref(0);
     
    function increment() {
        count.value ++
    }

    function decrement() {
        count.value --
    }

    function reset(){
        count.value = 0
    }

</script>