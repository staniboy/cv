<template>
  <div>
    <h3 class="text-lg font-medium">{{ props.title }}</h3>
    <h3 class="text-md">{{ props.subtitle }}</h3>
    <slot></slot>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
  subtitle: string
}>()
</script>
