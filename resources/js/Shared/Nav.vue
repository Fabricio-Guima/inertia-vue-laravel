<template>
    <nav>
        <ul>
            <li> <Link href="/" class="text-blue-500 hover:underline">Home</Link> </li>
            <li> <Link href="/users" class="text-blue-500 hover:underline">Users</Link> </li>
            <li> <Link href="/settings" class="text-blue-500 hover:underline">Settings</Link> </li>
            <li> <Link href="/logout" method="post" :data="{foo: 'bar'}" class="text-blue-500 hover:underline" as="button" >Logout</Link> </li>
        </ul>
    </nav>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';

</script>

<style lang="scss" scoped>

</style>
