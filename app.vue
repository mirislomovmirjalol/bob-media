<template>
  <div class="text-white">
    <img class="absolute" src="https://www.dnafilms.com/images/dna_bg_1.jpg?crc=4223266470" alt="">
    <NuxtPage class="backdrop-blur-xl"/>
  </div>
</template>

<style>
* {
  @apply transition-all duration-200 ease-in-out;
}

html {
  @apply bg-black
}

h1 {
  @apply text-4xl text-white;
}

h3 {
  @apply text-2xl font-medium;
}

p {
  @apply text-sm text-gray-300;
}

a {
  @apply hover:text-yellow-500;
}

.page-enter-active,
.page-leave-active {
  transition: all 0.4s;
}

.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}

iframe {
  @apply w-full;
}
</style>
