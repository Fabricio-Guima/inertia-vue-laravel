<template>
    <Link
    class="text-blue-500 hover:underline"
    :class="{ 'font-bold underline': props.active }">
    <slot />
    </Link>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';

const props = defineProps({
    active: Boolean,
});
</script>

<style lang="scss" scoped>

</style>
