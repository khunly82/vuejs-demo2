<script setup lang="ts">
const emit = defineEmits<{
    (e: 'click', response: boolean): void 
}>()
</script>
<template>
    <div class="card">
        <p>Souhaitez-vous procéder au changement ?</p>
        <button @click="$emit('click', true)">Oui</button>
        <button @click="$emit('click', false)">Non</button>
    </div>
</template>
<style scoped>
.card {
    border: 1px solid black;
    padding: 10px;
    width: 300px;
}
</style>