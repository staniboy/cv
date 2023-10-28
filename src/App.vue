<template>
  <div class="container mx-auto p-5 flex w-[1024px] bg-slate-50 text-slate-800">
    <!-- Main Content -->
    <div class="flex flex-col gap-6 basis-2/3">
      <div>
        <h1 class="text-3xl font-medium">Stanislav Vysotskiy</h1>
        <h2 class="text-md">Vue.js Frontend Developer</h2>
      </div>
      <resume-section title="Objective">
        Results-driven Computer Information Systems graduate with expertise in Vue.js, Nuxt.js, and
        Node.js. Seeking a remote front-end developer role to create innovative web solutions and
        collaborate with global teams.
      </resume-section>
      <resume-section title="Education">
        <section-item
          title="Associate's Degree in Computer Information Systems"
          subtitle="Portland Community College, Portland, OR, 2020"
        />
        <section-item title="Complete Vue Developer 2023" subtitle="Zero to Mastery, Udemy, 2023" />
      </resume-section>
      <resume-section title="Projects">
        <section-item title="Taskonaut">
          <p>
            An application that will help you organize your daily life and arrange all the tasks in
            the shelves. Built with Vuetify, Typescript, Vue Composition API and Firebase as
            back-end solution for DB and Auth.
          </p>
          <r-link title="Source" href="http://https://github.com/taskonaut/taskonaut" />
          -
          <r-link title="Demo" href="https://taskonaut.vercel.app" />
        </section-item>
        <section-item title="Music App">
          <p>
            Music App for sharing and playing your and other's music. Written with Vue 3 options
            API, Howler for audio playback and Tailwind CSS for styling. Utilizes Firebase for DB,
            file storage and Auth.
          </p>
          <r-link title="Source" href="https://github.com/staniboy/music_app" />
          -
          <r-link title="Demo" href="https://music-app-five-liart.vercel.app/" />
        </section-item>
        <section-item title="Car Trader">
          <p>
            Car trading platform based on Nuxt with Supabase PostgreSQL and auth. Using Vee-validate
            for form handling. Yup for front and back-end data validation. Prisma ODM for handling
            PostgreSQL.<br />
            <i>
              Please note that live demo is on free render.com hosting and might take a minute "to
              spin back up"
            </i>
          </p>
          <r-link title="Source" href="https://github.com/staniboy/cartrader" />
          -
          <r-link title="Demo" href="https://car-trader.onrender.com/" />
        </section-item>
      </resume-section>
    </div>
    <!-- Sidebar Content -->
    <div class="flex flex-col basis-1/3"></div>
  </div>
</template>
<script setup lang="ts">
import ResumeSection from './components/ResumeSection.vue'
import SectionItem from './components/SectionItem.vue'
import RLink from './components/ResumeLink.vue'
</script>
