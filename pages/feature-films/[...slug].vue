<script lang="ts" setup>
const route = useRoute();
const title = (route.params.slug[0]).replace(/-/g, ' ');
</script>

<template>
  <div class="min-h-screen">
    <BackButton :title="title.toString()"/>
    <div class="container mx-auto p-4">
      <div class="md:w-3/4 mx-auto">
        <ContentDoc/>
      </div>
    </div>
  </div>
</template>
