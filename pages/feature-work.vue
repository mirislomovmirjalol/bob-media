<template>
  <div class="w-full md:min-w-[30%] min-w-[90%] font-bold">
    <ContentList path="/feature-work">
      <template #default="{ list }">
        <NuxtLink v-for="item in list" :to="item._path" activeClass="active" class="hover:text-yellow-500 cursor-pointer">
          <h5 v-text="item.title"/>
        </NuxtLink>
      </template>
      <template #not-found>
        <p>No articles found.</p>
      </template>
    </ContentList>
  </div>
  <div class="w-full md:min-w-[30%] min-w-[90%] font-bold">
    <NuxtPage/>
  </div>
</template>
