<!-- -v-bind -> binds an attribute dynamically -->
 <!-- means Dynamically sets attribute on an element like (src, class, ref)  using vue variable -->
  <!-- syntax :attribute="expression" -->

  <template>
    <div>
        <img :src="imageUrl" alt="Dynamic image" />
        <p :class="textClass">Hello Vue!</p>
    </div>
  </template>

<script setup>
   import { ref } from 'vue';   

   const imageUrl = ref('https://placekitten.com/200/200');
   const textClass = ref('text-blue-500 font-bold');
</script>