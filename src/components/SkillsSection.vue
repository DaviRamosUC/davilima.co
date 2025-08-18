<template>
  <section class="py-20">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Hábilidades</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          As habilidades, ferramentas e tecnologias em que sou realmente bom:
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
import jsIcon from '@/assets/javascript.png'
import reactIcon from '@/assets/react.png'
import nodeIcon from '@/assets/nodejs.png'
import expressIcon from '@/assets/express.png'
import postIcon from '@/assets/postgrees.png'
import mongoIcon from '@/assets/mongodb.png'
import tailIcon from '@/assets/tailwindcss.png'
import gitIcon from '@/assets/git.png'
import phpIcon from '@/assets/php.png'
import laravelIcon from '@/assets/laravel.png'

export default {
  name: 'SkillsSection',
  components: {
    SkillCard
  },
  setup() {
    const skills = [
      { name: 'PHP', icon: phpIcon, color: 'yellow' },
      { name: 'Laravel', icon: laravelIcon, color: 'yellow' },
      { name: 'JavaScript', icon: jsIcon, color: 'yellow' },
      { name: 'React', icon: reactIcon, color: 'blue' },
      { name: 'Node.js', icon: nodeIcon, color: 'green' },
      { name: 'Express.js', icon: expressIcon, color: 'gray' },
      { name: 'PostgreSQL', icon: postIcon, color: 'blue' },
      { name: 'MongoDB', icon: mongoIcon, color: 'green' },
      { name: 'Tailwind', icon: tailIcon, color: 'cyan' },
      { name: 'Git', icon: gitIcon, color: 'orange' }
    ]

    return {
      skills
    }
  }
}
</script>
