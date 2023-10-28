<template>
  <div class="flex flex-col gap-1">
    <div>
      <h3 class="text-lg font-medium">{{ props.title }}</h3>
      <h3 v-if="props.subtitle" class="text-md text-slate-500">{{ props.subtitle }}</h3>
    </div>
    <div><slot></slot></div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
  subtitle?: string
}>()
</script>
