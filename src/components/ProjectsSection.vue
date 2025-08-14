<template>
  <section id="work" class="py-20">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Projetos</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          Alguns dos projetos notáveis que eu construí :
        </h2>
      </div>

      <div class="space-y-20">
        <ProjectCard
          v-for="(project, index) in projects"
          :key="project.id"
          :project="project"
          :reverse="index % 2 !== 0"
        />
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import ProjectCard from '@/components/ProjectCard.vue'

export default {
  name: 'ProjectsSection',
  components: {
    ProjectCard
  },
  setup() {
    const projects = [
      {
        id: 1,
        title: 'Portfólio',
        description: 'Um portfólio simples feito com Vue.js e TailwindCSS.',
        image: '/api/placeholder/600/400',
        tags: ['Vue.js', 'TailwindCSS'],
        liveUrl: 'https://davilima-six.vercel.app/',
        codeUrl: 'https://github.com/DaviRamosUC/davilima.co'
      }
    ]

    return {
      projects
    }
  }
}
</script>
