<template>
  <div class="container mx-auto px-4 lg:max-w-4xl py-12">
    <header-nav />
    <nuxt />
    <div class="text-center text-sm text-gray-500">
      Built with 💖 by
      <a
        class="text-blue-500 hover:text-blue-800"
        href="https://github.com/knazran"
      >knazran</a>
    </div>
  </div>
</template>

<script>
import HeaderNav from '~/components/HeaderNav.vue'
export default {
  components: {
    HeaderNav
  }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
</style>
