<template>
  <div class="text-white">
    <img alt="" class="absolute" src="https://www.dnafilms.com/images/dna_bg_1.jpg?crc=4223266470">
    <div class="min-h-screen backdrop-blur-xl">
      <div class="container mx-auto py-48 px-4 overflow-auto">
        <div class="flex flex-row flex-nowrap space-x-32 overflow-auto">
          <Navbar class="w-96"/>
          <NuxtPage/>
        </div>
      </div>
    </div>
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

iframe {
  @apply w-full;
}
</style>
