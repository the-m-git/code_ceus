<script setup>
import { RouterLink, RouterView } from "vue-router";
import Header from '../src/components/markup/Header.vue'
import Menu from '../src/components/markup/Menu.vue'
import {ref} from 'vue'
import BasicInput from '../src/components/basic/Input.vue'

const inputText = ref('zalupa')
</script>

<template>
  <Header></Header>
  <div class="flex justify-between">
    <Menu></Menu>
    <div class="pt-12 pl-96 h-screen w-full"><div class="p-4"><RouterView /></div></div>
    <div class="fixed z-90 top-20 right-0 w-96 h-96 bg-red-500 color-white">text:{{inputText}}<BasicInput v-model="inputText"></BasicInput></div>
  </div>
 
</template>