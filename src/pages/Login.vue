<script setup lang="ts">
import { useTitle } from '@vueuse/core';
import { RouterLink } from 'vue-router';
useTitle('Nerd.io | Login')
</script>
<template>
    <div class="w-full min-h-screen bg-slate-50 grid place-content-center pb-20">
        <div class="w-full md:w-[28rem] bg-white rounded-lg p-8">
            
            <h1 class="font-semibold text-xl">
                Welcome Back!
            </h1>
            <form class="w-full mt-8">

            <div class="flex flex-wrap -mx-3 mb-4">
                <div class="w-full px-3">
                <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-email">
                    Email Address
                </label>
                <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-email" type="email" placeholder="name@email.com">
                
                </div>
            </div>
     
            <div class="flex flex-wrap -mx-3 mb-4">
                <div class="w-full px-3">
                <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-password">
                    Password
                </label>
                <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-password" type="password" placeholder="Password">
              
                </div>
            </div>

            <div class="flex items-center justify-between mb-4">
                <div class="flex">
                    <input type="checkbox" name="remember" id="remember">
                    <label for="remember" class=" ml-2 inline-block align-baseline font-bold text-sm text-gray-700">Remember me</label>
                </div>
                <a class="inline-block align-baseline font-bold text-sm text-rose-500 hover:text-rose-800" href="#">
                    Forgot Password?
                </a>
            </div>

            
            <button class="w-full bg-rose-500 hover:bg-rose-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="button">
                Sign In
            </button>
           
    </form>
    <RouterLink :to="{ name: 'sign-up' }" class="block text-center mt-8">Don't have an account? <span class="text-rose-500">Register</span></RouterLink>
        </div>
    </div>
</template>
