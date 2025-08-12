<template>
  <section class="bg-white dark:bg-gray-800 py-20 transition-colors duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Experience</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          Here is a quick summary of my most recent experiences:
        </h2>
      </div>

      <div class="space-y-8">
        <ExperienceCard
          v-for="experience in experiences"
          :key="experience.id"
          :experience="experience"
        />
      </div>
    </div>
  </section>
</template>

<script lang="ts">
import ExperienceCard from '@/components/ExperienceCard.vue'

export default {
  name: 'ExperienceSection',
  components: {
    ExperienceCard
  },
  setup() {
    const experiences = [
      {
        id: 1,
        company: 'Wyvate',
        position: 'UX Designer',
        period: 'Nov 2021 - Present',
        logo: '🔥',
        responsibilities: [
          'Reviewed and designed UI for mobile demo app',
          'Worked with a team of 3 designers.',
          'Supported making IOS and ToS Design for Skouters'
        ]
      },
      {
        id: 2,
        company: 'Sense Original',
        position: 'UX Designer',
        period: 'Apr 2021 - Oct 2021',
        logo: '👁️',
        responsibilities: [
          'Designed Website for Sense Original',
          'Designed 5 ADVERT Applications that were a success.',
          'Organized a team of 2 to review ideas about designs being developed',
          'Collected 2 CSS Code along with 60 User Data collection and processing.'
        ]
      }
    ]

    return {
      experiences
    }
  }
}
</script>
