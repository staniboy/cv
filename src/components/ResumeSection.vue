<template>
  <div class="flex flex-col">
    <div class="relative flex gap-2 items-center">
      <div class="w-[16px] flex place-content-center">
        <font-awesome-icon :icon="`fa-solid ${props.icon}`" />
      </div>
      <div class="text-2xl font-medium">{{ props.title }}</div>
    </div>
    <div class="pl-[24px] py-2 flex flex-col gap-3"><slot></slot></div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps<{
  title: string
  icon: string
}>()
</script>
