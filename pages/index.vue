<template>
  <div class="my-8 lg:my-12">
    <h1 class="text-center text-2xl tracking-widest font-bold">FOOD BLOG</h1>
    <div class="my-8">
      <blog-card v-for="(blogPost, index) in blogPosts" :key="index" :blogPost="blogPost"></blog-card>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import BlogCard from '~/components/BlogCard.vue'

export default {
  components: {
    Logo,
    BlogCard
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
