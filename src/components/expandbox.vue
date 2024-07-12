<script setup>
import { ref } from 'vue';

const showContent = ref(false)
</script>

<template>
    <div>
        <button @click="showContent = !showContent">Mostrar</button>
            <div v-if="showContent == true" class="expandbox">aqui vai um texto escondido</div>
    </div>
</template>

<style scoped>

.expandbox {
    height: 100%;
    padding: 20px;
    border: 1px solid black;
    box-shadow: 2px 2px 3px 3px gray;
    border-radius: 10px;
}
</style>