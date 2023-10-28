<template>
  <div class="flex flex-col">
    <h2 class="text-2xl font-medium">{{ props.title }}</h2>
    <div class="py-2"><slot></slot></div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
}>()
</script>
