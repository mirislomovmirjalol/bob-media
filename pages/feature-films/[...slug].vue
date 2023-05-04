<script lang="ts" setup>
const title = "text";
</script>

<template>
  <div class="min-h-screen">
    <BackButton :title="title"/>
    <div class="container mx-auto p-4">
      <div class="md:w-3/4 mx-auto">
        <ContentDoc/>
      </div>
    </div>
  </div>
</template>
