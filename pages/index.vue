<template>
  <div>
    <header>
      <h1>Basic Nuxt Template</h1>
      <p>Get started faster</p>
    </header>
    <main>
      <section>
        <h2>Why US?</h2>
      </section>
    </main>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  head() {
    return {
      script: [{ src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }],
    };
  },
})
</script>

