<script setup>

import {ref} from "vue";

const warmWelcome = ref('Welcome to your new Laravel application.');

defineProps({
    laravelVersion: String,
    phpVersion: String,
});
</script>

<template>
    <div
        class="relative flex items-top justify-center min-h-screen bg-gray-100 dark:bg-gray-900 sm:items-center sm:pt-0">
        <div class="max-w-6xl mx-auto sm:px-6 lg:px-8">
            <div class="flex justify-center mt-4 sm:items-center sm:justify-between">
                <div class="ml-4 text-center text-base text-gray-500 sm:text-right sm:ml-0">
                    {{ warmWelcome }} Laravel v{{ laravelVersion }} (PHP v{{ phpVersion }})
                </div>
            </div>
        </div>
    </div>
</template>
