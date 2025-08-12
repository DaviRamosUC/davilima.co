<template>
  <section class="py-20">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Work</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          Some of the noteworthy projects I have built:
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
        title: 'Adays',
        description: 'CRAFTING WEBSITES THAT ELEVATE YOUR BRAND We transform your brand\'s vision into a reality, creating remarkable websites that engage users and drive sustainable business growth.',
        image: '/api/placeholder/600/400',
        tags: ['React', 'Next.js', 'TypeScript', 'TailwindCSS', 'PostgreSQL'],
        liveUrl: '#',
        codeUrl: '#'
      },
      {
        id: 2,
        title: 'Adays',
        description: 'CRAFTING WEBSITES THAT ELEVATE YOUR BRAND We transform your brand\'s vision into a reality, creating remarkable websites that engage users and drive sustainable business growth.',
        image: '/api/placeholder/600/400',
        tags: ['React', 'Next.js', 'TypeScript', 'TailwindCSS', 'PostgreSQL'],
        liveUrl: '#',
        codeUrl: '#'
      },
      {
        id: 3,
        title: 'Adays',
        description: 'CRAFTING WEBSITES THAT ELEVATE YOUR BRAND We transform your brand\'s vision into a reality, creating remarkable websites that engage users and drive sustainable business growth.',
        image: '/api/placeholder/600/400',
        tags: ['React', 'Next.js', 'TypeScript', 'TailwindCSS', 'PostgreSQL'],
        liveUrl: '#',
        codeUrl: '#'
      }
    ]

    return {
      projects
    }
  }
}
</script>
