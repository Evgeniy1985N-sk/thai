<script setup lang="ts">
  import { defineProps } from 'vue';

  const props = defineProps<{
    background: string;
  }>();
</script>

<template>
  <section class="intro" :style="{ backgroundImage: `url(${props.background})` }"></section>
</template>

<style lang="scss" scoped>
  @use '@/assets/components/Intro2.scss';
</style>