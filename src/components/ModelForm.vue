<template>
    <form>
        <input type="text" v-model="inputText">
        <br>
        <input type="checkbox" v-model="agree"> Acepto los terminos y condiciones
        <br>
        <select v-model="country">
            <option value="peru"> Perú </option>
            <option value="colombia"> Colombia </option>
            <option value="chile"> Chile </option>
        </select>
    </form>
    <h3>{{ inputText}}</h3>
</template>

<script lang="ts" setup>
    import {Ref, ref } from 'vue'
    let inputText:Ref<string> = ref('')
    let agree:Ref<boolean> = ref(true)
    let country:Ref<string> = ref('peru')
</script>

<style scoped></style>