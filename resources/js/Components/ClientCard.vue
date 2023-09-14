<script setup>
defineProps({
    client: Object
})
</script>

<template>
    <div class="min-w-[350px] mb-4 mx-2 p-4 bg-white rounded shadow border flex-1 cursor-pointer">
        <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
            {{ client.first_name }} {{ client.last_name }} 
        </h5>
        <hr class="mb-3">
        <ul class="list-disc space-y-2 px-4">
            <li>Level {{ client.level }}</li>
            <li>{{ client.address }}</li>
            <li>{{ client.phone }}</li>
        </ul>
    </div>
</template>