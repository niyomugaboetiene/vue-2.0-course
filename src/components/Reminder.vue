<template>
    <p>{{ count }}</p>
    <button @click="increment">+</button>
    <button @click="reset">0</button>
    <button @click="decrement">-</button>

    <p v-for="fruit in fruits">
        {{ fruit  }}
    </p>
        
       <p v-if="showGreeting === true">HelloVue</p>
        <p v-else>Click to greet</p>
        <button @click="greet">Greet</button>
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

const fruits = ref(["apple", "orange", "banana"]);

const showGreeting = ref(false);

function greet() {
    showGreeting.value = true
}

</script>