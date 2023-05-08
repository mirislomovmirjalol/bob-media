<script lang="ts" setup>
const links = [
  {
    name: 'Company',
    path: '/company',
  },
  {
    name: 'Our filming and production process',
    path: '/our-filming-and-production-process',
  },
  {
    name: 'Feature Work',
    path: '/feature-work',
  },
  {
    name: 'Event Promotional Videos',
    path: 'event-promotional-videos',
  },
  {
    name: 'Contact',
    path: '/contact',
  }
]
</script>

<template>
  <div class="min-w-fit">
    <div class="flex flex-col">
      <NuxtLink class="font-extrabold text-3xl" to="/">
        Logo
      </NuxtLink>

      <div class="my-24">
        <ul class="font-bold">
          <li v-for="link in links" class="my-2 text-xs md:text-base">
            <NuxtLink :to="link.path" activeClass="active">
              {{ link.name }}
            </NuxtLink>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style>
.active {
  color: #F59E0B;
}
</style>
