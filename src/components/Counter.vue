<template>
   <div class="ms-[700px] mt-[100px] p-7 shadow-2xl w-[16%] rounded-xl">
    <p class="text-center me-[30px] font-bold">{{ count }}</p>
    <div class="flex space-x-6">
        <button @click="increment" class="bg-blue-400 px-2 py-2 text-white rounded-lg hover:bg-blue-500 transition duration-200">Increment</button>
        <button @click="reset" class="bg-blue-400 px-2 py-2 text-white rounded-lg hover:bg-blue-500 transition duration-200">Reset</button>
        <button @click="decrement">Decrement</button>
    </div>
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
