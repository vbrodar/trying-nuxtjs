<template>
  <div>
    <Header />
    <Nuxt />
  </div>
</template>

<script>
import Header from './partials/Header'
export default {
  components: {
    Header,
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href: 'https://fonts.googleapis.com/css?family=Lato&display=swap',
        },
      ],
    }
  },
  mounted() {
    this.$nextTick(() => {
      this.$nuxt.$loading.start()

      setTimeout(() => this.$nuxt.$loading.finish(), 500)
    })
  },
}
</script>
<style lang="scss">
@use "../assets/main.scss";

html {
  font-family: 'Lato';
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  &,
  body {
    width: 100%;
    height: 100vh;
    padding: 0;
    margin: 0;
  }
}
</style>
