<template>
  <v-main>
    <h1>{{ gallery.title }}</h1>
    <ul>
      <li>Publish Date: {{ gallery.start }}</li>
      <li>Tags: {{ gallery.tags }}</li>
      <li>Image: <nuxt-img :src="gallery.image" /></li>
    </ul>
  </v-main>
</template>
<!-- JS export -->
<script>
export default {
     async asyncData({ $content, params, error }) {
    try {
      const gallery = await $content(`gallery/${params.slug}`).fetch()
      return {
        gallery,
      }
    } catch (e) {
      error('No article found')
    }
  },
}
</script>