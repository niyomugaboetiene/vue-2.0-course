<!-- -v-bind -> binds an attribute dynamically -->
 <!-- means Dynamically sets attribute on an element like (src, class, ref)  using vue variable -->
  <!-- syntax :attribute="expression" -->

  <template>
    <div>
        <img :src="imageUrl" alt="Dynamic image" />
        <p :class="textClass">Hello Vue!</p>
    </div>

    <!-- v-model -> is used to connect input to  vue variable so the UI updates to the variable and vice versa -->
     <!-- works for inputs, selects, textareas, checkboxes -->
      <input v-model="name" placeholder="Type your name here ..." />
      <p>Hello {{ name }}</p>

      <!-- v-if/v-else return the element if only the condition is true -->
       <!-- v-else if element is false -->
        <button @click="toggle">Toggle</button>
        <p v-if="showGreeting">Hello Vue</p>
       <p v-else>Good Bye</p>
  </template>

<script setup>
   import { ref } from 'vue';   

  //  const imageUrl = ref('https://placekitten.com/200/200');
  //  const textClass = ref('text-blue-500 font-bold');
  const showGreeting = ref(true);
  function toggle() {
    showGreeting.value = !showGreeting.value
  }
  const name = ref('');
</script>