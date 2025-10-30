<!-- interpolation is way of displaying daynamic data like (variable or expression) directly inside your HTML template -->
 <template>
    <div>
        <h1>{{  message  }}</h1>
        <p v-for="(fruit, index) in fruits">
            {{ index + 1 }} . {{ fruit }}
        </p>
    </div>
 </template>

 <script setup>
     import { ref } from 'vue';
     
     const message = ref("Hello vue 3!"); // ~ this one act as state in react js

   const fruits = ref(["Apple", "Mango", "Banana", "Pineaple"])
</script>