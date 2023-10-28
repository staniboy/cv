<template>
  <div>
    <h3 class="text-lg font-medium">{{ props.title }}</h3>
    <h3 v-if="props.subtitle" class="text-md mb-4 text-slate-500">{{ props.subtitle }}</h3>
    <slot></slot>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
  subtitle?: string
}>()
</script>
