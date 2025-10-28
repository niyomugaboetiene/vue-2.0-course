<template>
   <div class="ms-[700px] mt-[100px] p-7 shadow-2xl w-[20%] rounded-xl">
    <p class="text-center me-[10px] font-bold mb-6">{{ count }}</p>
    <div class="flex space-x-6 ms-4">
        <button @click="increment" class="bg-blue-400 px-2 py-2 text-white rounded-lg hover:bg-blue-500 transition duration-200">Increment</button>
        <button @click="reset" class="bg-red-400 px-2 py-2 text-white rounded-lg hover:bg-red-500 transition duration-200">Reset</button>
        <button @click="decrement" class="bg-green-400 px-2 py-2 text-white rounded-lg hover:bg-green-500 transition duration-200">Decrement</button>
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
