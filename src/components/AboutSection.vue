<template>
  <section id="about" class="bg-white dark:bg-gray-800 py-20 transition-colors duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide">Sobre mim</p>
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
            Curioso sobre mim?
          </h2>

          <div class="space-y-4 text-gray-600 dark:text-gray-300 leading-relaxed">
            <p>
              I'm a passionate, self-proclaimed designer who specializes in full stack development (React.js & Node.js). I am very enthusiastic about bringing the technical and visual aspects of digital products to life. User experience, pixel perfect design, and writing clear, readable, highly performant code matters to me.
            </p>

            <p>
              Comecei minha jornada como desenvolvedor web em 2015 e desde então, continuei a crescer e evoluir como desenvolvedor, enfrentando novos desafios e aprendendo as tecnologias mais recentes pelo caminho.
            </p>

            <p>
              Eu tenho um pensamento progressista e gosto de trabalhar em produtos desde a ideia até o desenvolvimento.
            </p>

            <p>Finalmente, alguns dados pessoais sobre mim:</p>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-4 mt-6">
              <ul class="space-y-2">
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Bacharel em Engenharia de Software
                </li>
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Autodidata
                </li>
              </ul>
              <ul class="space-y-2">
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Desenvolvedor Full Stack
                </li>
                <li class="flex items-center">
                  <span class="w-2 h-2 bg-blue-600 dark:bg-blue-400 rounded-full mr-3"></span>
                  Foco no ecossistema PHP (Laravel, Symfony) e Vue.js
                </li>
              </ul>
            </div>

            <p class="pt-4">
              E mais uma coisa, eu estou disponivel para trabalhar como freelancer, então sinta-se livre para entrar em contato e dizer olá! 😉
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
