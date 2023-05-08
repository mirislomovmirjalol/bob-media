<script lang="ts" setup>
const route = useRoute();
const title = (route.params.slug[0]).replace(/-/g, ' ');
</script>

<template>
  <ContentDoc/>
</template>
