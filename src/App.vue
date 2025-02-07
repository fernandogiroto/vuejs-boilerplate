<template>
  <router-view v-slot="{ Component }">
    <transition :name="'fade'" mode="out-in">
      <component :is="Component" :key="Component" />
    </transition>
  </router-view>
</template>

<script setup lang="ts">
</script> 

<style>
  @import '@/scss/theme.scss';
</style>
