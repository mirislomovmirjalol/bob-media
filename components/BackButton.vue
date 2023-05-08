<script lang="ts" setup>
const props = defineProps({
  title: String,
});
</script>

<template>
  <div>
    <div class="text-white">
      <nav
          class="
          container
          px-6
          py-8
          mx-auto
          flex justify-between items-center
        "
      >
        <NuxtLink to="/feature-work" class="p-2 rounded-full border border-white hover:scale-[0.8] hover:text-white">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5"
               stroke="currentColor" class="w-6 h-6">
            <path stroke-linecap="round" stroke-linejoin="round" d="M10.5 19.5L3 12m0 0l7.5-7.5M3 12h18"/>
          </svg>
        </NuxtLink>

        <h3 class="capitalize">
          {{ title }}
        </h3>
        <span/>
      </nav>
    </div>
  </div>
</template>

<style scoped></style>
