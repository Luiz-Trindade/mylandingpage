<script lang="ts" setup>
interface TimelineItem {
    opposite: string;
    title: string;
    description: string;
}

defineProps({
    timelineItems: {
        type: Array as PropType<TimelineItem[]>,
        default: () => [
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
    },
});
</script>

<template>
    <v-container>
        <v-timeline align="start">
            <v-timeline-item v-for="(item, index) in timelineItems" :key="index">
                <template #opposite>
                    {{ item.opposite }}
                </template>
                <div>
                    <div class="text-h6">{{ item.title }}</div>
                    <p>{{ item.description }}</p>
                </div>
            </v-timeline-item>
        </v-timeline>
    </v-container>
</template>

<style scoped></style>
