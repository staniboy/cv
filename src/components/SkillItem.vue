<template>
  <div>
    <div class="text-md pb-1">{{ props.title }}</div>
    <div class="w-full h-1 bg-slate-200">
      <div class="h-1 bg-green-600" :style="{ width: `${percent}%` }"></div>
    </div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
  percent: number
}>()
</script>
