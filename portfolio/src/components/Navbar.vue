<template>
    <div class="flex h-screen">
        <nav class="bg-gray-800 text-white w-32 p-4 flex flex-col items-center" ref="navbar">
            <ul class="space-y-20 pt-12">
                <li>
                    <homeicon />
                </li>
                <li>
                    <personicon />
                </li>
                <li>
                    <homeicon />
                </li>

            </ul>
        </nav>
    </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue';
import { gsap } from 'gsap';
import homeicon from './icons/homeicon.vue';
import personicon from './icons/personicon.vue';

const navbar = ref(null);

onMounted(() => {
    const tl = gsap.timeline();
    tl.from(navbar.value, { duration: 2, x: -100, opacity: 0, ease: 'power3.out' });
});
</script>

<style scoped>
/* Add any additional styles here */
</style>
