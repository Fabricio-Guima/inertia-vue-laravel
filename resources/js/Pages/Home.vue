<template>
    <Head title="Home" />
    <div>
        <h1>Hello, {{ props.name }}</h1>

        <h2>Stacks:</h2>
        <ul>
        <li v-for="framework in props.frameworks" :key="framework">{{ framework }}</li>
        </ul>
    </div>
</template>

<script setup>
import { Head, Link } from '@inertiajs/vue3';
const props = defineProps({
    name: String,
    frameworks: Array
});
</script>

<style lang="scss" scoped>

</style>
