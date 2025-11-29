<script lang="ts" setup>
const AppHeroProps = ref({
  title: 'Luiz Trindade - Desenvolvedor de software',
  subtitle: 'Transformando ideias em soluções digitais',
  description: 'Olá! Sou Luiz Trindade, um desenvolvedor de software apaixonado por criar soluções digitais inovadoras. Com experiência em diversas tecnologias, estou sempre em busca de novos desafios para transformar ideias em realidade. Meu objetivo é entregar produtos de alta qualidade que atendam às necessidades dos clientes, utilizando as melhores práticas de desenvolvimento e mantendo-me atualizado com as tendências do mercado.',
  backgroundImage: 'https://wallpaperaccess.com/full/314785.jpg',
  image: 'https://luiz-trindade-dev.netlify.app/assets/profile_picture-D4iy5gfz.png',
});

// const AppPortifolioProps = ref({
//   title: 'Our Portfolio',
//   subtitle: 'Showcasing Our Best Work',
//   description: 'Explore a curated selection of our most impactful projects that demonstrate our commitment to excellence, innovation, and client satisfaction.',
//   backgroundImage: 'https://cdn.vuetifyjs.com/docs/images/cards/dark-beach.jpg',
//   image: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg',
// });

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
  title: 'Luiz Trindade - Desenvolvedor de software',
  ogTitle: 'Luiz Trindade - Desenvolvedor de software',
  description: 'Olá! Sou Luiz Trindade, um desenvolvedor de software apaixonado por criar soluções digitais inovadoras. Com experiência em diversas tecnologias, estou sempre em busca de novos desafios para transformar ideias em realidade. Meu objetivo é entregar produtos de alta qualidade que atendam às necessidades dos clientes, utilizando as melhores práticas de desenvolvimento e mantendo-me atualizado com as tendências do mercado.',
  ogDescription: 'Olá! Sou Luiz Trindade, um desenvolvedor de software apaixonado por criar soluções digitais inovadoras. Com experiência em diversas tecnologias, estou sempre em busca de novos desafios para transformar ideias em realidade. Meu objetivo é entregar produtos de alta qualidade que atendam às necessidades dos clientes, utilizando as melhores práticas de desenvolvimento e mantendo-me atualizado com as tendências do mercado.',
});
</script>

<template>
  <div>
    <AppHero v-bind="AppHeroProps" />
    <!-- <AppPortifolio v-bind="AppPortifolioProps" /> -->
    <AppTimeline v-bind="AppTimelineProps" />
    <AppContact />
  </div>
</template>

<style scoped></style>