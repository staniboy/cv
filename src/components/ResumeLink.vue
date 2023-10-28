<template>
  <a :href="props.href" class="text-lime-700 font-medium">{{ title }}</a>
</template>
<script setup lang="ts">
const props = defineProps<{
  href: string
  title: string
}>()
</script>
