<template>
  <div class="flex flex-col items-center text-center group">
    <div class="w-16 h-16 flex items-center justify-center text-3xl mb-3 group-hover:scale-110 transition-transform duration-200">
      {{ skill.icon }}
    </div>
    <span class="text-sm font-medium text-gray-700 dark:text-gray-300">{{ skill.name }}</span>
  </div>
</template>

<script lang="ts">
export default {
  name: 'SkillCard',
  props: {
    skill: {
      type: Object,
      required: true
    }
  }
}
</script>
