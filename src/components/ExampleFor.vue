<template>
    <ul>
        <li v-for=" country in countries" v-bind:key="country.code">{{ country.name }} </li>
    </ul>
</template>

<script lang="ts" setup>
    import {Ref, ref} from 'vue'
    interface Country {
        code: string,
        name: string
    }
    let countries:Ref<Array<Country>> = ref([
        {
            code: 'pe',
            name: 'Perú'
        },
        {
            code: 'chi',
            name: 'Chile'
        },
        {
            code: 'col',
            name: 'Colombia'
        },
        {
            code: 'bra',
            name: 'Brasil'
        }
    ])
</script>

<style scoped>
    ul{
        list-style: none;
    }
</style>