<template>
  <section class="py-20">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Skills</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          The skills, tools and technologies I am really good at:
        </h2>
      </div>

      <div class="grid grid-cols-3 md:grid-cols-4 lg:grid-cols-5 xl:grid-cols-9 gap-8">
        <SkillCard
          v-for="skill in skills"
          :key="skill.name"
          :skill="skill"
        />
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import SkillCard from '@/components/SkillCard.vue'

export default {
  name: 'SkillsSection',
  components: {
    SkillCard
  },
  setup() {
    const skills = [
      { name: 'JavaScript', icon: '🟨', color: 'yellow' },
      { name: 'Figma', icon: '🎨', color: 'purple' },
      { name: 'React', icon: '⚛️', color: 'blue' },
      { name: 'Node.js', icon: '💚', color: 'green' },
      { name: 'Express.js', icon: '⚡', color: 'gray' },
      { name: 'PostgreSQL', icon: '🐘', color: 'blue' },
      { name: 'MongoDB', icon: '🍃', color: 'green' },
      { name: 'Socket.io', icon: '🔌', color: 'black' },
      { name: 'Tailwind', icon: '🎨', color: 'cyan' },
      { name: 'Git', icon: '📝', color: 'orange' }
    ]

    return {
      skills
    }
  }
}
</script>
