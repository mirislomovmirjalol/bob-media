<template>
  <div class="text-white">
    <img alt="" class="absolute" src="https://www.dnafilms.com/images/dna_bg_1.jpg?crc=4223266470">
    <div class="min-h-screen backdrop-blur-xl">
      <div class="container mx-auto py-48 px-4 overflow-auto">
        <div class="flex flex-row flex-nowrap md:space-x-32 space-x-12 overflow-auto">
          <Navbar />
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
  @apply md:text-4xl text-xl text-white;
}

h3 {
  @apply text-2xl font-medium;
}

h5 {
  @apply md:text-base text-xs font-medium;
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
