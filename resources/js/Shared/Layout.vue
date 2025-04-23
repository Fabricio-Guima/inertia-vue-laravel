<template>
    <section class="p-6 bg-gray-200">
        <header class="flex items-center justify-between">
            <div class="flex items-center">
                <h1 class="font-bold text-lg">My App</h1>

                <p class="text-sm ml-4">Welcome, {{ username }}</p>
            </div>

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
import { computed } from "vue";
import Nav from "./Nav.vue";

const username = computed(() => $page.props.auth.user.name);



</script>

<style scoped>

</style>
