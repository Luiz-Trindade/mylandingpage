<script lang="ts" setup></script>

<template>
    <v-app-bar class="appBar" :elevation="4">
        <template #prepend>
            <v-app-bar-nav-icon />
        </template>

        <v-app-bar-title>Application Bar</v-app-bar-title>
    </v-app-bar>
</template>

<style scoped>
.appBar {
    background-color: rgba(255, 255, 255, 0.8);
    backdrop-filter: blur(8px);
}
</style>