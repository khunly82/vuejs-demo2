<script setup lang="ts">
import { defineModel, defineProps } from 'vue';
const {message} = defineProps<{message: string}>();
const visible = defineModel<boolean>('visible', { required: true });
</script>
<template>
<div class="alert" v-if="visible">
    <div class="top">
        <span @click="visible = false">&times</span>
    </div>
    <p>{{ message }}</p>
</div>
</template>
<style scoped>
.alert {
    border: 1px solid red;
    background-color: rgb(252, 202, 202);
    color: red;
    font-weight: bold;
    padding: 10px;
    width: 300px;
    margin-top: 20px;
    border-radius: 5px;
    .top {
        text-align: right;
        span {
            cursor: pointer;
        }
    }
}
</style>