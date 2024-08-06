<template>
    <h1>hELLO</h1> 
  
  {{ name }}



  <input type="text" v-model="name" @input="handleUpdate">
</template>


<script setup>
    import { ref } from 'vue';


    const emit  = difineEmits(['updateName'])



    const handleUpdate = (event) => {
        console.log(event.target.value);
        
    }


    const name = ref('')
</script>



