
<!-- <script setup lang="js">
import PropsChild from './Props/propsChild.vue';

</script>

<template>
  <PropsChild name="Etiene"/>
</template> -->

<template>
  <PropsChild :name="username" />
</template>

<script>
import PropsChild from './propsChild.vue';

export default {
   components: { PropsChild },
   data() {
    return {
      username: 'Etiene'
    }
   }
}

</script>