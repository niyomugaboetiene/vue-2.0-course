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

        <p v-if="count > 5">This {{ count }} is too big</p>
        <p v-if="count === 3">This count is exactly</p>
        <p v-if="count < 3">{{ count }} is too small</p>
        <button @click="increaseCOunt">Increase COunt</button>


        <!-- v-for is used to loop over list dynamically -->
         <li v-for="(fruit, index ) in fruits" key="index">
          {{  index + 1 }} . {{ fruit }}
         </li>

         <!-- v-on is used to DOM events ataching an event listener to an element -->
         <!-- v-on:eventName="methoodName" --> <br>
         <button @click="sayHello">Click Me</button> <br>
         <div class="ms-3 shadow-lg w-[200px] mt-4 p-4 rounded-lg">
             <button @click="counted ++">You clicked {{ counted }} timees</button>
         </div>
  </template>

<script setup>
   import { ref } from 'vue';   

  //  const imageUrl = ref('https://placekitten.com/200/200');
  //  const textClass = ref('text-blue-500 font-bold');
  // const showGreeting = ref(true);
  // const count = ref(1);
  // const fruits = ref(["Apple", "Orange", "Banana"]);

  // function increaseCOunt() {
  //   count.value ++;
  // }
  // function toggle() {
  //   showGreeting.value = !showGreeting.value
  // }
  // const name = ref('');
  function sayHello() {
    alert("Hello vue");
  }
  
  const counted = ref(0);
</script>