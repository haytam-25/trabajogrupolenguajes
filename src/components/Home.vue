<script setup>
import {defineProps} from 'vue';

const props = defineProps({
    sTitulo:{
        type: String,
        default: 'TITULO APP'
    }
});

</script>

<template>

<h1> {{sTitulo}} </h1>


</template>

<style scoped>



</style>
