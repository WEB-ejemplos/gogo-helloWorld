<template>
    <h1>V-ON</h1>
    <p :style="{
        backgroundColor: 'blue',
        color : c
    }">Mensajeeeeeeeee</p>
    <button @:click="handleClick()">Cambiar Color</button>
</template>

<script lang="ts" setup>
    import { ref } from 'vue'
    let c = ref('#fff')
    const handleClick = () => {
        c.value = '#ff0000'
    }
</script>

<style scoped>
</style>