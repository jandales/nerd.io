<script setup lang="ts">
import { useTitle } from '@vueuse/core';
import { RouterLink } from 'vue-router';
useTitle('Nerd.io | Page not Found')
</script>

<template>
        <div class="container flex flex-col items-center justify-center px-5 mx-auto pt-24 pb-16">
                    <div class="max-w-md text-center">
                        <h2 class="mb-8 font-extrabold text-9xl text-rose-500">
                            <span class="sr-only">Error</span>404
                        </h2>
                        <p class="text-2xl font-semibold md:text-3xl text-gray-400">Sorry, we couldn't find this page.</p>
                        <p class="mt-4 mb-8 text-gray-400">But don't worry, you can find plenty of other things on our homepage.</p>
                        <RouterLink rel="noopener noreferrer" :to="{name : 'home'}" class="px-8 py-3 font-semibold rounded bg-rose-500 text-white">Back to homepage</RouterLink>
                    </div>
                </div>
</template>
