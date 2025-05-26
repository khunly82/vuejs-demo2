<script setup lang="ts">
import { defineProps } from 'vue';
const name = defineProps<{name: string}>();
</script>
<template>
    <p>Hello {{name}} !!</p>
</template>
<style scoped></style>