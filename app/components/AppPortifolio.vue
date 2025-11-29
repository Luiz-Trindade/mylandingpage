<script setup lang="ts">
// Define props for the component
const props = defineProps({
    title: {
        type: String,
        default: 'Default Title',
    },
    subtitle: {
        type: String,
        default: 'Default Subtitle',
    },
    description: {
        type: String,
        default: 'This is a default description for the AppHero component.',
    }
});

// SEO Meta Tags
useSeoMeta({
    title: props.title,
    ogTitle: props.title,
    description: props.description,
    ogDescription: props.description,
});
</script>

<template>
    <!-- eslint-disable-next-line vue/first-attribute-linebreak -->
    <v-card class="fade-enter-active pa-6 hero-card" color="surface-variant" :title="title" :subtitle="subtitle"
        rounded="0">
        <h1>Olá</h1>
    </v-card>
</template>

<style scoped></style>