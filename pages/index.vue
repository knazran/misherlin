<template>
  <div class="my-8 lg:my-12">
    <h1 class="text-center text-2xl tracking-widest font-bold">FOOD BLOG</h1>
    <div>
      <ul v-for="(blogPost, index) in blogPosts" :key="index">
        <nuxt-link :to="`blog/${blogPost.slug}`">{{blogPost.title}}</nuxt-link>
        <p>{{blogPost.description}}</p>
      </ul>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  },
  head() {
    return {
      script: [
        { src: 'https://identity.netlify.com/v1/netlify-identity-widget.js' }
      ]
    }
  },
  computed: {
    blogPosts() {
      return this.$store.state.blogPosts
    }
  }
}
</script>

<style>
</style>
