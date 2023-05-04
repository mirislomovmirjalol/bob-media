<script lang="ts" setup xmlns:x-transition="http://www.w3.org/1999/xhtml">
const showMenu = ref(false);
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
          md:flex md:justify-between md:items-center
          border-b border-white
        "
      >
        <div class="flex items-center justify-between">
          <NuxtLink to="/">
            Logo
          </NuxtLink>
          <!-- Mobile menu button -->
          <div @click="showMenu = !showMenu" class="flex md:hidden">
            <button
                type="button"
            >
              <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                <path
                    fill-rule="evenodd"
                    d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
                ></path>
              </svg>
            </button>
          </div>
        </div>


        <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
        <ul
            :class="showMenu ? 'flex' : 'hidden'"
            class="
            flex-col
            mt-8
            space-y-4
            md:flex
            md:space-y-0
            md:flex-row
            md:items-center
            md:space-x-10
            md:mt-0
          "
        >
          <NuxtLink to="/company" class="text-sm cursor-pointer">
            Company
          </NuxtLink>
          <NuxtLink to="/feature-films" class="text-sm cursor-pointer">
            Feature Films
          </NuxtLink>
          <NuxtLink to="/contact" class="text-sm cursor-pointer">
            Contact
          </NuxtLink>
          <NuxtLink to="/team" class="text-sm cursor-pointer">
            Team
          </NuxtLink>
        </ul>
      </nav>
    </div>
  </div>
</template>

<style scoped></style>
