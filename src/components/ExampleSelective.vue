<template>
    <h1 v-if=" age < 18 ">Eres menor de Edad</h1>
    <h1 v-else>Eres mayor de Edad</h1>
</template>

<script lang="ts" setup>
    let age =18

</script>

<style scoped></style>