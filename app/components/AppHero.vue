<script lang="ts" setup>
// Define component props with default values
defineProps({
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
    },
    backgroundImage: {
        type: String,
        default: 'https://cdn.vuetifyjs.com/docs/images/cards/dark-beach.jpg',
    },
    image: {
        type: String,
        default: 'https://cdn.vuetifyjs.com/images/cards/sunshine.jpg',
    },
});
</script>

<template>
    <!-- eslint-disable-next-line vue/first-attribute-linebreak -->
    <v-card class="fade-enter-active pa-6 hero-card" color="surface-variant" :title="title" :subtitle="subtitle"
        :image="backgroundImage" rounded="0">
        <v-row>
            <!-- Coluna de texto: ocupa 12 colunas (100%) em mobile, 6 colunas (50%) em md+ -->
            <v-col cols="12" md="8" class="d-flex flex-column justify-center align-center" order="2" order-md="1">
                <p class="text-body-1 text-md-h6 pa-6">{{ description }}</p>
            </v-col>

            <!-- Coluna de imagem: ocupa 12 colunas (100%) em mobile, 6 colunas (50%) em md+ -->
            <v-col cols="12" md="4" class="d-flex flex-column justify-center align-center" order="1" order-md="2">
                <v-avatar :image="image" size="225" />
            </v-col>
        </v-row>
    </v-card>
</template>

<style scoped>
.hero-card {
    position: relative;
    overflow: hidden;
    min-height: 70vh;
}

.hero-card :deep(.v-card__image) {
    filter: blur(8px) brightness(35%);
}

.hero-card :deep(.v-row) {
    position: relative;
    z-index: 1;
}

/* Ajustes de padding para mobile */
@media (max-width: 959px) {
    .hero-card {
        padding: 1rem !important;
    }
}
</style>