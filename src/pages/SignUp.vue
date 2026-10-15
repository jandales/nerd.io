<script setup lang="ts">
import { useTitle } from '@vueuse/core';
import { RouterLink } from 'vue-router';
useTitle('Nerd.io | Sign-up')
</script>
<template>
    <div class="w-full min-h-screen bg-slate-50 grid place-content-center pb-20">
        <div class="w-full md:w-[28rem] bg-white rounded-lg p-8">
            <h1 class="font-semibold text-xl">
               Create an Account
            </h1>
            <form class="w-full  mt-8">

            <div class="flex flex-wrap -mx-3 mb-4">
                <div class="w-full px-3">
                <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-name">
                    Name
                </label>
                <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-name" type="text" placeholder="Name">
            
                </div>
            </div>

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

            <div class="flex flex-wrap -mx-3 mb-4">
                    <div class="w-full px-3">
                    <label class="block uppercase tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-confirm-password">
                        Confirm Password
                    </label>
                    <input class="appearance-none block w-full bg-gray-200 text-gray-700 border border-gray-200 rounded py-3 px-4 mb-3 leading-tight focus:outline-none focus:bg-white focus:border-gray-500" id="grid-confirm-password" type="password" placeholder="Confirm password">
              
                    </div>
                </div>

          
            <button class="w-full bg-rose-500 hover:bg-rose-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline" type="button">
                Sign Up
            </button>
           
    </form>
     <RouterLink :to="{ name: 'login' }"  class="block text-center mt-8">Have an account? <span class="text-rose-500">Sign-in</span></RouterLink>
        </div>
    </div>
</template>
