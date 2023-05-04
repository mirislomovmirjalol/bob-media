<template>
  <div class="min-h-screen">
    <Navbar/>
    <div class="container mx-auto p-4">
      <ContentList path="/feature-films">
        <template #default="{ list }">
          <NuxtLink v-for="item in list" :to="item._path" class="hover:text-yellow-500 cursor-pointer">
            <h3 v-text="item.title"/>
          </NuxtLink>
        </template>
        <template #not-found>
          <p>No articles found.</p>
        </template>
      </ContentList>
    </div>
  </div>
</template>
