<template>
    <div class="pt-16">
        <h1 class="text-3xl font-semibold mb-4">Ihnat ride</h1>
        <div class="overflow-hidden shadow sm:rounded-md max-w-sm mx-auto text-left">
            <div class="bg-white px-4 py-5 sm:p-6"></div>
            <div class="flex justify-between text-white">
                <button class="rounded-md border border-transperent bg-black py-2 px-4 text-sm font-medium">
                    Start driving
                </button>
                <button @click="handleFindaRide" class="rounded-md border border-transperent bg-black py-2 px-4 text-sm font-medium">
                    Find a ride
                </button>
            </div>
        </div>
    </div>
</template>

<script setup>
import { useRouter } from 'vue-router';

const router  = useRouter()
const handleFindaRide = () => {
    router.push({
        name: 'location'
    })
}
</script>