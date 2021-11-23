<template>
  <v-main>
    <v-container>
      <h1>{{ fave.tags }}</h1>
      <p>{{ fave.description }}</p>
    </v-container>
  </v-main> 
</template>

<!-- JS Export -->
<script>
export default {
     async asyncData({ $content, params, error }) {
    try {
      const fave = await $content(`favourites/${params.slug}`).fetch()
      return {
        fave,
      }
    } catch (e) {
      error('No article found')
    }
  },
}
</script>