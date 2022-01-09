<template>
  <v-app>

    <Header></Header>

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <Footer></Footer>

  </v-app>
</template>

<script>
export default {
  name: 'default',
  data () {
    return {
    }
  },
  methods: {
    onScroll() {
      this.$scrollTo('#target')
    }
  },
  mounted () {
    const hash = this.$route.hash
    if (hash && hash.match(/^#.+$/)) {
      this.$scrollTo(hash)
    }
  }
}
</script>

<style lang="scss" scoped>

</style>
