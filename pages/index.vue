<template>
<div>
  <!-- blog -->
  <v-container>
    <h1>My blog</h1>
    <ul>
      <li v-for="blog in blogs" :key="blog.slug">
        <NuxtLink :to="`blog/${blog.slug}`"> {{ blog.title }}</NuxtLink>
      </li>
    </ul>
  </v-container>

  <!-- favourites -->
  <v-container>
    <h2>Favourites</h2>
    <ul>
      <li v-for="fave in faves" :key="fave.slug">
        <NuxtLink :to="`favourites/${fave.slug}`"> {{ fave.tags }} </NuxtLink>
      </li>
    </ul>
  </v-container>

  <!-- gallery -->
  <v-container>
    <h3>Gallery</h3>
    <ul>
      <li v-for="gallery in galleries" :key="gallery.slug">
        <NuxtLink :to="`gallery/${gallery.slug}`"> {{ gallery.title }} </NuxtLink>
      </li>
    </ul>
  </v-container>

</div>
</template>
<!-- JS export -->
<script>
export default {
  async asyncData({ $content }) {
    const blogs = await $content('blog').fetch()
    const faves = await $content('favourites').fetch()
    const galleries = await $content('gallery').fetch()

    return {
      blogs,
      faves,
      galleries,
    }
  },
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' },
      ],
    }
  },
}
</script>
