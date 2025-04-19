<template>
    <Head title="Users" />
    <div>
        <h1 class="text-3xl">Users Page</h1>
    </div>
    <Nav />
    <div style="margin-top: 800px;">
        <p>The current time is {{ time }}.</p>

        <Link href="/users" class="text-blue-500 hover:underline" preserve-scroll>Refresh</Link>
    </div>
</template>

<script setup>
import { Head, Link } from '@inertiajs/vue3';
import Nav from '../Shared/Nav.vue';

const props = defineProps({
    time: String,
});

</script>

<style lang="scss" scoped>

</style>
