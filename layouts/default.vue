<template>
  <v-app>
    <header>
      <v-app-bar
        id="top"
        color="indigo darken-1"
        dark
        fixed
        app
      >
        <nuxt-link to="/">
          <v-toolbar-title class="white--text">BarCodeSystems</v-toolbar-title>
        </nuxt-link>

        <v-spacer></v-spacer>

        <v-btn
          small
          text
        >
          <nuxt-link v-scroll-to="'#philosophy'" to class="white--text mr-2">経営理念</nuxt-link>
        </v-btn>

        <v-btn
          small
          text
        >
          <nuxt-link v-scroll-to="'#works'" to class="white--text mr-2">リリース実績</nuxt-link>
        </v-btn>

        <v-btn
          small
          text
        >
          <nuxt-link v-scroll-to="'#target'" to class="white--text mr-2">content3</nuxt-link>
        </v-btn>

        <v-btn
          small
          text
        >
          <nuxt-link v-scroll-to="'#target'" to class="white--text mr-2">content4</nuxt-link>
        </v-btn>

        <nuxt-link to="/contact" class="mr-2">
          <v-btn
            small
            text
          >
            お問い合わせ
          </v-btn>
        </nuxt-link>

      </v-app-bar>
    </header>

    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer
      color="green accent-4" dark
      app
    >
      <span class="mr-2">&copy; 2021</span>
      <span>BarCodeSystems</span>
    </v-footer>

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
