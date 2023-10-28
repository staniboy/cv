<template>
  <div class="container mx-auto p-5 flex flex-col gap-4 w-[1024px] bg-slate-50">
    <div>
      <h1 class="text-3xl font-medium">Stanislav Vysotskiy</h1>
      <h2 class="text-md">Vue.js Frontend Developer</h2>
    </div>

    <resume-section title="Education">
      <section-item
        title="Associate's Degree in Computer Information Systems"
        subtitle="Portland Community College, Portland, OR, 2020"
      >
        Graduated with Web Application Development, Java Application Programming, Database Design
        and SQL Certifications.
      </section-item>
    </resume-section>
  </div>
</template>
<script setup lang="ts">
import ResumeSection from './components/ResumeSection.vue'
import SectionItem from './components/SectionItem.vue'
</script>
