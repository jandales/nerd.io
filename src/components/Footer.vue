<script setup lang="ts">
import { RouterLink } from 'vue-router';
</script>
<template>
    <footer class=" bg-slate-50">
        <div class="container mx-auto py-10 px-8 flex justify-center items-center">
            <nav class="flex flex-col gap-8">
                <ul class="flex flex-wrap justify-center gap-6 sm:gap-10">
                    <li><RouterLink :to="{name :'home'}" class="text-slate-600 hover:text-rose-500">Home</RouterLink></li>
                    <li><RouterLink :to="{name :'faq'}" class="text-slate-600 hover:text-rose-500">FAQ</RouterLink></li>
                    <li><RouterLink :to="{name :'privacy-policy'}" class="text-slate-600 hover:text-rose-500">Privacy Policy</RouterLink></li>
                </ul>
                <span class="block text-center text-slate-600">© Nerd.io</span>
            </nav>
        </div>
    </footer>
</template>
