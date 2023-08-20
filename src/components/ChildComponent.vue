<script setup>
import { defineProps } from 'vue';

defineProps(['person', 'messageToChild', 'messageFromChild'])
defineEmits(['update:messsageFromChild'])
</script>
<template>
    <div class="p-5 border-2 border-gray-300 border-s-fuchsia-50">
        <div class="max-w-lg mx-auto p-4 bg-white rounded-md shadow-md flex flex-col items-center justify-center mb-5">
            <!-- <h1 class="text-xl font-bold text-gray-900">
                {{ messageToChild }}
            </h1> -->
        </div>

        <div class="max-w-md mx-auto p-10 bg-white rounded-md shadow-md flex flex-col items-center justify-center">
            <img class="w-20 h-20 rounded-full ring-4 ring-sky-600" src="https://media.geeksforgeeks.org/wp-content/cdn-uploads/20220131222755/Vue.js-Tutorial.png" alt="Vue Js ">
            <div class="flex flex-col items-center justify-center pt-5 pb-5">
                <p class="text-lg font-semibold">{{ person.name }}</p>
                <p class="text-sm text-gray-500">{{ person.title }}</p>
            </div>
        </div>
    </div>
</template>