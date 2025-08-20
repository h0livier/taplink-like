<script setup lang="ts">
interface BrandLink{
    title: string
    text: string
    link: string
}
const props = defineProps<BrandLink>()
</script>
<template>
    <div class="mb-3 p-2 border-2 rounded-md border-blue-500">
        <NuxtLink :href="props.link">
            <div class="flex items-center">
                <div class="grow">
                    <p class="text-lg text-blue-500">{{ props.title }}</p>
                    <p class=" text-gray-300">{{ props.text }}</p>
                </div>
            </div>
        </NuxtLink>  
    </div>
</template>