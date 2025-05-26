<script setup lang="ts">
import { ref } from 'vue';
const name = ref<string>('Khun');
</script>
<template>
    <p>Hello {{name}} !!</p>
</template>
<style scoped></style>