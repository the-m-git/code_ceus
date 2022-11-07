<script setup>
import { RouterLink, RouterView } from "vue-router";
import Header from '../src/components/markup/Header.vue'
import Menu from '../src/components/markup/Menu.vue'
</script>

<template>
  <Header></Header>
  <div class="flex justify-between">
    <Menu></Menu>
    <div class="pt-12 pl-96 h-screen w-full"><div class="p-4"><RouterView /></div></div>
  </div>
 
</template>