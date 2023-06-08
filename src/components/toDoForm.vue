<script setup>
import { ref } from 'vue'

const event = ref({
    id: 1,
    category: 'Tame',
    title: 'Tame a Yutyrannus',
    date: '7th July 2023',
    deadline: '8th July 2023',
    requestor: 'Alex',
})
</script>

<template>
    <div class="flex flex-col">
        <div class="grid grid-cols-[100px_500px_210px] bg-white/10 rounded-md my-5 p-5 border-2 border-emerald-500 shadow-lg shadow-emerald-500/50 text-white hover:bg-emerald-200/10">
            <img :src="`src/assets/images/${event.category}Icon.png`" class="col-start-1 aspect-square w-[100px]">

            <div class="col-start-2 ml-5">
                <h2 class="text-emerald-500">{{ event.date }}</h2>
                <h2>{{ event.requestor }} requests: {{ event.title }}</h2>
                <h2 class="text-emerald-500">{{ event.description }}</h2>
            </div>
            
            <div class="flex items-center">
                <button class="col-start-3 w-[200px] h-[50px] justify-self-center bg-red-500 rounded-md p-2 hover:bg-red-900"> Mark as completed </button>
            </div>
        </div>
        
        <button class="w-[200px] bg-emerald-500 rounded-lg p-3 my-5 text-white hover:bg-emerald-800">ADD NEW ITEM</button>
    </div>
</template>

<style scoped></style>