<template>
  <div :class="{ 'dark': darkMode }" class="min-h-screen transition-colors duration-300">
    <div class="bg-gray-50 dark:bg-gray-900 min-h-screen">
      <!-- Navigation -->
      <NavBar @toggle-dark-mode="toggleDarkMode" :dark-mode="darkMode" />

      <!-- Hero Section -->
      <HeroSection />

      <!-- About Section -->
      <AboutSection />

      <!-- Skills Section -->
      <SkillsSection />

      <!-- Experience Section -->
      <ExperienceSection />

      <!-- Projects Section -->
      <ProjectsSection />

      <!-- Footer -->
      <FooterSection />
    </div>
  </div>
</template>

<script lang="ts">
import { ref, onMounted } from 'vue'
import NavBar from '@/components/Navbar.vue'
import HeroSection from '@/components/HeroSection.vue'
import AboutSection from '@/components/AboutSection.vue'
import SkillsSection from '@/components/SkillsSection.vue'
import ExperienceSection from '@/components/ExperienceSection.vue'
import ProjectsSection from '@/components/ProjectsSection.vue'
import FooterSection from '@/components/FooterSection.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    HeroSection,
    AboutSection,
    SkillsSection,
    ExperienceSection,
    ProjectsSection,
    FooterSection
  },
  setup() {
    const darkMode = ref(false)

    const toggleDarkMode = () => {
      darkMode.value = !darkMode.value
      localStorage.setItem('darkMode', darkMode.value)
    }

    onMounted(() => {
      const savedDarkMode = localStorage.getItem('darkMode')
      if (savedDarkMode !== null) {
        darkMode.value = JSON.parse(savedDarkMode)
      }
    })

    return {
      darkMode,
      toggleDarkMode
    }
  }
}
</script>
