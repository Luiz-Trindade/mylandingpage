<script lang="ts" setup>
defineProps({
    backgroundColor: {
        type: String,
        default: 'primary',
    },
})
</script>

<template>
    <v-container>
        <v-card :color="backgroundColor" class="pa-6 elevation-4" rounded="xl">
            <h1>Contato</h1>
        </v-card>
    </v-container>
</template>

<style scoped></style>