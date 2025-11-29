<script lang="ts" setup>
import ProfilePicture from '@/assets/profile_picture.png';
import BackGroundImage from '@/assets/background_image.jpg';

const AppHeroProps = ref({
  title: 'Luiz Trindade - Desenvolvedor de software',
  subtitle: 'Transformando ideias em soluções digitais',
  description: 'Olá! Sou Luiz Trindade, um desenvolvedor de software apaixonado por criar soluções digitais inovadoras. Com experiência em diversas tecnologias, estou sempre em busca de novos desafios para transformar ideias em realidade. Meu objetivo é entregar produtos de alta qualidade que atendam às necessidades dos clientes, utilizando as melhores práticas de desenvolvimento e mantendo-me atualizado com as tendências do mercado.',
  backgroundImage: BackGroundImage,
  image: ProfilePicture,
});

const AppTimelineProps = ref({
  timelineItems: [
    {
      opposite: '2020',
      title: 'Started Learning Vue.js',
      description: 'Began my journey into Vue.js and built my first small projects.',
    },
    {
      opposite: '2021',
      title: 'Built My First Vue App',
      description: 'Developed a full-fledged Vue.js application and deployed it online.',
    },
    {
      opposite: '2022',
      title: 'Contributed to Open Source',
      description: 'Started contributing to open source Vue.js projects on GitHub.',
    },
  ],
});

useSeoMeta({
  title: 'Luiz Trindade | Desenvolvedor Fullstack - Belém, PA',
  description: 'Desenvolvedor de Software Fullstack em Belém do Pará. Especialista em Vue.js, Nuxt e soluções Node.js. Foco em inovação, alta performance e desenvolvimento ágil.',
  keywords: 'Luiz Trindade, Desenvolvedor Fullstack, Full-Stack, Software Developer, Vue.js, Nuxt.js, Node.js, JavaScript, TypeScript, Belém do Pará, Pará, Brasil, Dev Web, Frontend, Backend, UI/UX, API REST, Banco de Dados, SQL, NoSQL, Soluções Digitais, Desenvolvimento Ágil, Portfólio, Contratação, Freela',
  robots: 'index, follow',
  author: 'Luiz Trindade',
  ogTitle: 'Luiz Trindade - Desenvolvedor Fullstack (Vue, Nuxt, Node)',
  ogDescription: 'Portfólio de Luiz Trindade, Fullstack Developer em Belém/PA. Veja projetos com Vue.js, Nuxt.js e Node.js.',
  ogUrl: 'https://luiz-trindade-dev.netlify.app/',
  ogType: 'website',
  // ogImage: 'https://luiz-trindade-dev.netlify.app/profile_picture.png',
  twitterCard: 'summary_large_image',
  twitterTitle: 'Luiz Trindade - Fullstack Expert',
  twitterDescription: 'Dev Fullstack em Belém do Pará. Contrate para projetos com foco em performance e qualidade de código.',
  // twitterImage: 'https://luiz-trindade-dev.netlify.app/profile_picture.png',
});
</script>

<template>
  <div>
    <AppHero v-bind="AppHeroProps" />
    <AppTimeline v-bind="AppTimelineProps" />
    <AppContact />
  </div>
</template>

<style scoped></style>