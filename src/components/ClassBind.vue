<template>
    <p :class="{
        'danger': hasError
    }
    ">El mensaje se envió satisfactoriamente</p>

    <p :style="{
        backgroundColor: '#ccc',
        color : hasError ? '' : 'blue'
    }">Estooo</p>

</template>

<script lang="ts" setup>
    let hasError = true
</script>

<style scoped>
    .danger{
        color: red;
    }
</style>