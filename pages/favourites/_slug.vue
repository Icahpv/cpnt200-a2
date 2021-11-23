<template>
  <v-main>
    <v-container>
      <h1>{{ fave.title }}</h1>
      <ul>
        <li>Publish Date: {{ fave.start }}</li>
        <li>Tags: {{ fave.tags }}</li>
      </ul>
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