<script lang="ts" setup>
const systemTheme = ref('light');
</script>

<template>
  <v-app :theme="systemTheme">
    <AppBar />

    <v-main>
      <slot />
    </v-main>

    <AppFooter />
  </v-app>
</template>

<style>
h1, h2, h3, h4, h5, h6 {
  font-family: Serif;
  font-size: 5em;
  text-align: center;
  text-shadow: 2px 4px 6px rgba(0, 0, 0, 0.3);
}

p {
  font-size: 1.2em;
  margin: 20px;
}

/* Fade In */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s;
}

.fade-enter,
.fade-leave-to {
  opacity: 0;
}

/* Slide In */
.slide-enter-active,
.slide-leave-active {
  transition: transform 0.5s;
}

.slide-enter {
  transform: translateX(100%);
}

.slide-leave-to {
  transform: translateX(-100%);
}

/* Scale In */
.scale-enter-active,
.scale-leave-active {
  transition: transform 0.5s;
}

.scale-enter {
  transform: scale(0);
}

.scale-leave-to {
  transform: scale(0);
}

/* Rotate In */
.rotate-enter-active,
.rotate-leave-active {
  transition: transform 0.5s;
}

.rotate-enter {
  transform: rotate(-180deg);
}

.rotate-leave-to {
  transform: rotate(180deg);
}
</style>