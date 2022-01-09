<template>
  <v-row class="text-center" justify="center" align="center">
    <v-col cols="12">
      トップページ-HP
      <font-awesome-icon icon="download"/>
      <font-awesome-icon icon="anchor"/>
      <font-awesome-icon icon="star"/>
      <font-awesome-icon :icon="['far', 'star']"  />
      <font-awesome-icon :icon="['fas', 'star']"  />
      <font-awesome-icon :icon="['fab', 'twitter']"  />
      <font-awesome-icon :icon="['far', 'star']"  />
      <font-awesome-icon :icon="['fas', 'download']"  />
    </v-col>
    <v-col cols="12">
      <Test></Test>
    </v-col>
    <v-col cols="12">
      <div style="height: 1000px">bg-color</div>
    </v-col>
    <v-col id="target" class="mt-16">
      <nuxt-link v-scroll-to="'#top'" to class="mr-2">トップへ</nuxt-link>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'index',
  methods: {

  }
}
</script>
