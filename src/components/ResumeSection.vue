<template>
  <div class="flex flex-col">
    <h2 class="text-2xl font-medium">{{ props.title }}</h2>
    <slot></slot>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
}>()
</script>
