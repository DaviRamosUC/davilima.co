<template>
  <section class="bg-white dark:bg-gray-800 py-20 transition-colors duration-300">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <p class="text-sm font-medium text-blue-600 dark:text-blue-400 uppercase tracking-wide mb-4">Experiência</p>
        <h2 class="text-2xl font-bold text-gray-900 dark:text-white">
          Aqui está um resumo rápido das minhas experiências mais recentes:
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
        company: 'Libre Soluções de Governo',
        position: 'Backend Developer | PHP | Vue.js | Laravel',
        period: 'Abr 2022 - Atualmente',
        logo: '💻',
        responsibilities: [
          'Liderei uma equipe de 4 desenvolvedores juniores no setor de Recursos Humanos, fornecendo orientação técnica e mentoria.',
          'Coordenei o desenvolvimento e a manutenção do sistema de gestão municipal E-Cidade e sua API de integração com o E-Social.',
          'Desenvolvi e mantive vários projetos Laravel e sistemas legados, garantindo sua contínua funcionalidade e estabilidade.',
          'Gerenciei diversas tarefas de DevOps relacionadas a Docker, Kubernetes e GitLab, otimizando processos de implantação e melhorando a eficiência da infraestrutura.',
          'Migrei projetos do sistema de gestão municipal E-Cidade para versões mais modernas do PHP (7.4/8.1), resultando em desempenho aprimorado e maior segurança.',
          'Utilizei PHP (5.6, 7.4, 8.1), Laravel, Docker, PostgreSQL, GitLab, PHPUnit e Kubernetes para construir, implantar e manter aplicações.',
          'Automatizei pipelines de implantação usando Docker e Kubernetes, reduzindo o tempo de implantação e minimizando a intervenção manual.',
          'Solucionei e resolvi problemas de produção relacionados a Docker, Kubernetes e GitLab, minimizando o tempo de inatividade.',
          'Colaborei com equipes multifuncionais para integrar novos recursos e melhorar sistemas existentes, resultando em um aumento na satisfação dos usuários.',
        ]
      },
      {
        id: 2,
        company: 'Libre Soluções de Governo',
        position: 'Estagiário de engenharia de software',
        period: 'Fev 2022 - Abr 2022',
        logo: '👨🏽‍💻',
        responsibilities: [
          'Durante meu período de estágio na Libre Soluções, aprimorei minhas habilidades, especialmente na comunicação e no desenvolvimento de software. Atuei na manutenção do sistema de gestão pública E-Cidade (software livre), realizando correções de bugs e implementando melhorias. Além disso, desenvolvi features, contribuindo para a evolução da plataforma e aprimorando meu conhecimento em desenvolvimento de software.'
        ]
      }
    ]

    return {
      experiences
    }
  }
}
</script>
