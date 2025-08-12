<template>
  <div class="bg-gray-50 dark:bg-gray-700/50 rounded-xl p-8 transition-colors duration-300">
    <div class="flex flex-col lg:flex-row gap-8">
      <div class="flex-shrink-0">
        <div class="w-16 h-16 bg-white dark:bg-gray-600 rounded-lg flex items-center justify-center text-2xl shadow-md">
          {{ experience.logo }}
        </div>
      </div>

      <div class="flex-1">
        <div class="flex flex-col lg:flex-row lg:justify-between lg:items-start mb-4">
          <div>
            <h3 class="text-xl font-semibold text-gray-900 dark:text-white">{{ experience.position }}</h3>
            <p class="text-gray-600 dark:text-gray-300 font-medium">{{ experience.company }}</p>
          </div>
          <span class="text-sm text-gray-500 dark:text-gray-400 mt-2 lg:mt-0">{{ experience.period }}</span>
        </div>

        <ul class="space-y-2">
          <li
            v-for="responsibility in experience.responsibilities"
            :key="responsibility"
            class="text-gray-600 dark:text-gray-300 flex items-start"
          >
            <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3 mt-2 flex-shrink-0"></span>
            {{ responsibility }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'ExperienceCard',
  props: {
    experience: {
      type: Object,
      required: true
    }
  }
}
</script>
