<template>
  <section id="about" class="bg-white dark:bg-gray-800 py-20 transition-colors duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide">About me</p>
      </div>

      <div class="flex flex-col lg:flex-row gap-12 items-center">
        <div class="flex-shrink-0">
          <!-- <img
            src="/api/placeholder/400/500"
            alt="Rishabh working"
            class="w-80 h-96 object-cover rounded-2xl shadow-lg"
          /> -->
        </div>

        <div class="flex-1">
          <h2 class="text-3xl font-bold text-gray-900 dark:text-white mb-6">
            Curious about me? Here you have it:
          </h2>

          <div class="space-y-4 text-gray-600 dark:text-gray-300 leading-relaxed">
            <p>
              I'm a passionate, self-proclaimed designer who specializes in full stack development (React.js & Node.js). I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User experience, pixel perfect design, and writing clear, readable, highly performant code matters to me.
            </p>

            <p>
              I began my journey as a web developer in 2015, and since then, I've continued to grow and evolve as a developer, taking on new challenges and learning the latest technologies along the way.
            </p>

            <p>
              I am very much a progressive thinker and enjoy working on products end to end, from ideation all the way to development.
            </p>

            <p>
              When I'm not in full-on developer mode, you can find me hovering around on twitter or on indie hacker, witnessing the journey of early startups or enjoying some free time. You can follow me on Twitter where I share tech-related bites and build in public, or you can follow me on GitHub.
            </p>

            <p>Finally, some quick bits about me:</p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-6">
              <ul class="space-y-2">
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  B.E. in Computer Engineering
                </li>
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Avid learner
                </li>
              </ul>
              <ul class="space-y-2">
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Full time freelancer
                </li>
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  UI Designer
                </li>
              </ul>
            </div>

            <p class="pt-4">
              One last thing, I'm available for freelance work, so feel free to reach out and say hello! I promise I don't bite 😉
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts">
export default {
  name: 'AboutSection'
}
</script>
