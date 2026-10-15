<script setup lang="ts">
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
</script>

<template>
    <Header />
    <div class="pt-20 lg:pt-24 min-h-screen">
      <router-view></router-view>
    </div>
    <Footer />
</template>

<style scoped>
</style>
