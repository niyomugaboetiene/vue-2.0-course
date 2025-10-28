<!-- interpolation is way of displaying daynamic data like (variable or expression) directly inside your HTML template -->
 <template>
    <div>
        <h1>{{  message  }}</h1>
    </div>
 </template>

 <script setup>
     import { ref } from 'vue';
     
     const message = ref("Hello vue 3!");

</script>