<template>
<Hello />

 


<br>
<br>
<input type="text" v-model="name">
<input type="text" v-model="age">

</template>

<script setup>
  import Hello from  './components/Hello.vue'
  import { watch, ref } from 'vue';

  
  const name = ref( 'Mamoudou' )
  const age = ref( '26' )

  watch(name, (newValue, oldValue) => {
    console.log(newValue, oldValue);
    
  })
</script>



<style scoped>

  .bold {
    font-weight: bolder;
  }

  .text-red {
    color: indianred;
  }

  .text-green {
    color: green;
  }
</style>
