<script setup lang="ts">
import Confirm from './components/Confirm.vue';
const log = console.log;
</script>

<template>
    <Confirm @click="e => log(e)"></Confirm>
</template>

<style scoped>
</style>
