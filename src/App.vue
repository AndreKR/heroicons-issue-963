<template>
  <a v-for="item in navigation">
    <div><component :is="item.icon" /> {{ item.name }}</div>
  </a>
</template>

<script setup lang="ts">
  import { HomeIcon } from '@heroicons/vue/24/outline';
  
  let navigation = [
    {icon: HomeIcon, name: 'Home'}
  ];
</script>