<template>
    edit {{route.params.index}}
</template>


<script setup>
import {useRoute} from 'vue-router';

const route =  useRoute();
console.log(route.params)
const props = defineProps(['index'])


</script>

