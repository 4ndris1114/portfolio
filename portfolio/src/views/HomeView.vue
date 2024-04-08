<script setup lang="ts">
import Navbar from '@/components/Navbar.vue';
</script>

<template>
  <div class="flex">
    <Navbar />
    <div class="flex-1">
      <div class="wrapperdiv">
        <h1 class="text-2xl text-center pt-4">Welcome to My Portfolio</h1>
        <div class="container mx-auto flex flex-wrap mt-10">
          <div class="max-w-4xl p-6 bg-slate-200 rounded-lg">
            <p class="text-gray-700 leading-relaxed text-xl">Lorem ipsum dolor sit amet, consectetur adipiscing elit.
              Cras sit amet euismod sapien. Ut in libero molestie eros luctus fringilla. Donec tincidunt id augue sit
              amet elementum. Proin sit amet nunc turpis. Quisque quis urna et augue porta pellentesque. Cras eget orci
              non velit fermentum venenatis. Nullam varius vehicula elit et rhoncus.</p>
          </div>
          <div class="flex justify-end">
            <img class="w-4/5 rounded-3xl shadow-md" src="@/assets/portrait.jpeg" alt="My Image">
          </div>
        </div>
      </div>
    </div>
  </div>
</template>