<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Aumentar</button>
</template>

<script lang="ts" setup>
import { defineComponent, Ref, ref } from "vue";

let counter: Ref = ref(0);
const addCounter = (): void => {
    counter.value++;
};
</script>

<style scoped></style>
