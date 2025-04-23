<template>
    <section class="p-6 bg-gray-200">
        <header class="flex items-center justify-between">
            <h1 class="font-bold text-lg">My App</h1>
            <Nav />
        </header>
    </section>

    <section class="p-6">
        <div class="max-w-3xl mx-auto">
            <slot />
        </div>
    </section>
</template>

<script setup lang="ts">
import Nav from "./Nav.vue";

</script>

<style scoped>

</style>
