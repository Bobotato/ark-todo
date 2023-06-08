<script setup>
import toDoItem from '../components/toDoItem.vue'
import toDoForm from '../components/toDoForm.vue'
</script>

<template> 
  <body class="h-screen bg-[#181818] pt-2">
    <button class="w-[200px] bg-emerald-500 rounded-lg p-3 my-5 text-white hover:bg-emerald-800">ADD NEW ITEM</button>
    <toDoForm></toDoForm>
    <div class="flex flex-col items-center">
      <toDoItem></toDoItem>
      <toDoItem></toDoItem>
    </div>
  </body>
</template>