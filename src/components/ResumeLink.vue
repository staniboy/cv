<template>
  <a :href="props.href" class="text-green-600 hover:text-green-800 font-medium cursor-pointer">
    {{ title }}
  </a>
</template>
<script setup lang="ts">
const props = defineProps<{
  href: string
  title: string
}>()
</script>
