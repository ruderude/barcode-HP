<template>
  <div>
    <header>
      <v-app-bar
        id="top"
        color="indigo darken-1"
        dark
        fixed
        app
      >

        <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>

        <nuxt-link to="/">
          <v-toolbar-title class="white--text">BarCodeSystems</v-toolbar-title>
        </nuxt-link>

        <v-spacer></v-spacer>

        <v-tabs right>
          <v-tab
            v-for="(item, index) in menuItems"
            :key="index"
          >
            <nuxt-link :to="item.url" class="white--text">{{ item.name }}</nuxt-link>
          </v-tab>
        </v-tabs>

      </v-app-bar>

      <v-navigation-drawer
        v-model="drawer"
        fixed
        temporary
      >
        <v-list
          nav
          dense
        >
          <v-list-item-group>
            <v-list-item
              v-for="(item, index) in menuItems"
              :key="index"
            >
              <v-list-item-title>
                <nuxt-link :to="item.url" class="grey--text text--darken-4">{{ item.name }}</nuxt-link>
              </v-list-item-title>
            </v-list-item>

          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
    </header>
  </div>
</template>

<script>
export default {
  name: 'header_d',
  data () {
    return {
      drawer: false,
      menuItems: [
        {
          name: '経営理念',
          url: '/#philosophy'
        },
        {
          name: 'リリース実績',
          url: '/#works'
        },
        {
          name: '代表挨拶',
          url: '/#representative'
        },
        {
          name: 'お問い合わせ',
          url: '/contact'
        },
      ]
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
.v-app-bar__nav-icon {
  @include display_pc {
    display: none !important;
  }
}

.v-tabs {
  display: none;

  @include display_pc {
    display: block !important;
  }
}
</style>
