<template>
  <div class="page main-content">
    <NavBar />
    <main>
      <Nuxt />
      <ShareButton :title="'Basic Template'" :description="'This is a description'" />
    </main>
    <footer class="center-text">
      <div class="bi-column">
        <div class="column-start">
          <NuxtLink to="/">Home</NuxtLink>
          <NuxtLink to="/">Products</NuxtLink>
          <NuxtLink to="/">Contact Us</NuxtLink>
        </div>
        <div class="column-end">
          <a href="">
            <img width="40" height="40" src="~/assets/images/facebook.svg" alt="Facebook Logo">
          </a>
          <a href="">
            <img width="40" height="40" src="~/assets/images/instagram.svg" alt="Instagram Logo">
          </a>
        </div>
      </div>
      &copy; 2020 Knight Digital Development 
    </footer>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import ShareButton from '~/components/ShareButton.vue'
import NavBar from '~/components/NavBar.vue'

export default Vue.extend({
  components: { ShareButton, NavBar }
})
</script>

<style scoped>
.main-content {
  max-width: 900px;
  margin: 0 auto;
}
main {
  padding: var(--pad);
}
</style>

