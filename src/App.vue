<template>
  <div class="container mx-auto p-10 w-[1024px] bg-slate-50 text-slate-800">
    <div class="pb-5">
      <h1 class="text-4xl font-medium mb-2">Stanislav Vysotskiy</h1>
      <h2 class="text-md">Vue.js Frontend Developer</h2>
    </div>
    <div class="flex gap-4">
      <!-- Main Content -->
      <div class="flex flex-col gap-6 basis-3/4">
        <resume-section title="Objective">
          Results-driven Computer Information Systems graduate with expertise in Vue.js, Nuxt.js,
          and Node.js. Seeking a remote front-end developer role to create innovative web solutions
          and collaborate with global teams.
        </resume-section>
        <resume-section title="Education">
          <section-item
            title="Associate's Degree in Computer Information Systems"
            subtitle="Portland Community College, Portland, OR, 2020"
          />
          <section-item
            title="Complete Vue Developer 2023"
            subtitle="Zero to Mastery, Udemy, 2023"
          />
        </resume-section>
        <resume-section title="Projects">
          <section-item v-for="project in projects" :key="project.name" :title="project.name">
            <p>
              {{ project.description }}
            </p>
            <span class="text-sm">
              <r-link title="Source" :href="project.source" />
              -
              <r-link title="Demo" :href="project.demo" />
            </span>
          </section-item>
        </resume-section>
      </div>
      <!-- Sidebar Content -->
      <div class="flex flex-col basis-1/4 gap-8">
        <section-item title="Details">
          <span>(415) 895-0361</span>
          <r-link title="stanley.v@outlook.com" href="mailto:stanley.v@outlook.com" />
        </section-item>
        <section-item title="Links">
          <r-link title="Github" href="https://github.com/staniboy" />
          <r-link title="LinkedIn" href="https://www.linkedin.com/in/staniboy" />
        </section-item>
        <section-item title="Languages">
          <skill title="English" :percent="80" />
          <skill title="Russian" :percent="100" />
        </section-item>
        <section-item title="Technical Skills">
          <skill
            v-for="skill in skills"
            :key="skill.name"
            :title="skill.name"
            :percent="skill.percent"
          ></skill>
        </section-item>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import ResumeSection from './components/ResumeSection.vue'
import SectionItem from './components/SectionItem.vue'
import RLink from './components/ResumeLink.vue'
import Skill from './components/SkillItem.vue'

const projects = [
  {
    name: 'Taskonaut',
    description:
      'An application that will help you organize your daily life and arrange all the tasks in the shelves. Built with Vuetify, Typescript, Vue Composition API and Firebase as back-end solution for DB and Auth.',
    source: 'http://https://github.com/taskonaut/taskonaut',
    demo: 'https://taskonaut.vercel.app'
  },
  {
    name: 'Music App',
    description:
      "Music App for sharing and playing your and other's music. Written with Vue 3 options API, Howler for audio playback and Tailwind CSS for styling. Utilizes Firebase for DB, file storage and Auth.",
    source: 'https://github.com/staniboy/music_app',
    demo: 'https://music-app-five-liart.vercel.app'
  },
  {
    name: 'Cartrader',
    description:
      'Car trading platform based on Nuxt with Supabase PostgreSQL and auth. Using Vee-validate for form handling. Yup for front and back-end data validation. Prisma ODM for handling PostgreSQL.',
    source: 'https://github.com/staniboy/cartrader',
    demo: 'https://car-trader.onrender.com'
  }
]
const skills = [
  {
    name: 'Vue.js',
    percent: 95
  },
  {
    name: 'JavaScript',
    percent: 95
  },
  {
    name: 'Vuetify',
    percent: 75
  },
  {
    name: 'Tailwind CSS',
    percent: 90
  },
  {
    name: 'NPM',
    percent: 80
  },
  {
    name: 'Git',
    percent: 70
  },
  {
    name: 'Rest API',
    percent: 75
  },
  {
    name: 'TypeScript',
    percent: 60
  },
  {
    name: 'Node.js',
    percent: 60
  }
]
</script>
