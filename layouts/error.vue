<template>
  <div class="center-text">
    <h1 v-if="error.statusCode === 404">Page Not Found</h1>
    <h1 v-else>An Error Occurred</h1>
    <NuxtLink to="/">Home page</NuxtLink>
  </div>
</template>

<script>
export default {
  props: ['error'],
  validate({ query }) {
    if (query.preview) {
      return true
  }},
}
</script>
