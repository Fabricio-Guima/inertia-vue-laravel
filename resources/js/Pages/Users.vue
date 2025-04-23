<template>
    <Layout>

        <Head title="Users" />
        <div>
            <h1 class="text-3xl">Users Page</h1>
        </div>

        <div style="margin-top: 800px;">
            <p>The current time is {{ time }}.</p>

            <Link href="/users" class="text-blue-500 hover:underline" preserve-scroll>Refresh</Link>
        </div>

    </Layout>
</template>

<script setup>
import { Head } from '@inertiajs/vue3';
import Layout from '../Shared/Layout.vue';

const props = defineProps({
    time: String,
});

</script>

<style lang="scss" scoped>

</style>
