<template>
  <v-row class="text-center" justify="center" align="center">
    <v-col class="pa-0" cols="12">
      <v-parallax
        dark
        :src="topImage"
      >
        <v-overlay
          absolute
          color="#fff"
        >
          <v-row
            align="center"
            justify="center"
          >
            <v-col
              class="text-left ml-6"
              cols="12"
            >
              <h1 class="grey--text text--darken-4 text-h3 font-weight-bold mb-4">
                Bar Code Systems
              </h1>
              <h4 class="grey--text text--darken-3 text-h5 font-weight-bold">
                納得あるこだわりを
              </h4>
            </v-col>
          </v-row>
        </v-overlay>
      </v-parallax>
    </v-col>

    <v-col id="philosophy" class="bg_1 pa-16" cols="12">
      <div>
        <h1 class="indigo--text text--darken-4 text-h4 font-weight-bold mb-4">
          経営理念
        </h1>
        <h4 class="indigo--text text--darken-4 text-h6 font-weight-bold">
          お客様の心に寄り添うhogehoge
        </h4>
      </div>
      <v-row justify="center" align="center">
        <v-col cols="12" sm="6">
          <v-img
            :src="philosophyImage"
          ></v-img>
        </v-col>
        <v-col cols="12" sm="6">
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
          テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
        </v-col>
      </v-row>
    </v-col>

    <v-col id="works" class="bg_2 pa-16" cols="12">
      <div>
        <h1 class="indigo--text text--darken-4 text-h4 font-weight-bold mb-4">
          リリース実績
        </h1>
      </div>
      <div class="mb-6">
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
      </div>

      <v-row justify="center" align="center">
        <v-col cols="12" sm="4">
          <v-card>
            <v-img
              :src="worksImage1"
            ></v-img>

            <v-divider class="mx-4"></v-divider>

            <v-card-title class="indigo--text text--darken-4">タップ de アンケート</v-card-title>

            <v-card-text>
              <div class="text-left">
                ユーザービリティを追求し、ユーザーが回答しやすいアンケートフォームを作成することにより企業が欲する顧客データを高い精度で取得します。
              </div>
            </v-card-text>

          </v-card>
        </v-col>

        <v-col cols="12" sm="4">
          <v-card>
            <v-img
              :src="worksImage2"
            ></v-img>

            <v-divider class="mx-4"></v-divider>

            <v-card-title class="indigo--text text--darken-4">かしかん！</v-card-title>

            <v-card-text>
              <div class="text-left">
                ビル看板を借りたい人と貸したい人のマッチングサービスです。地図検索や条件検索により、ユーザーの要望に適した看板を見つけることが可能です。
              </div>
            </v-card-text>

          </v-card>
        </v-col>

        <v-col cols="12" sm="4">
          <v-card>
            <v-img
              :src="worksImage3"
            ></v-img>

            <v-divider class="mx-4"></v-divider>

            <v-card-title class="indigo--text text--darken-4">Day3tasks</v-card-title>

            <v-card-text>
              <div class="text-left">
                To C向けのタスク管理ツールです。LINE Messaging APIを使って、実装したアプリケーションであるためLINE上で友達追加するだけで使えます。
              </div>
            </v-card-text>

          </v-card>
        </v-col>

      </v-row>
    </v-col>

    <v-col cols="12">
      <Test></Test>
      <v-card
        :loading="loading"
        class="mx-auto my-12"
        max-width="374"
      >
        <template slot="progress">
          <v-progress-linear
            color="deep-purple"
            height="10"
            indeterminate
          ></v-progress-linear>
        </template>

        <v-img
          height="250"
          :src="image_src"
        ></v-img>

        <v-card-title class="test">Bar Code</v-card-title>

        <v-card-text>
          <v-row
            align="center"
            class="mx-0"
          >
            <v-rating
              :value="4.5"
              color="amber"
              dense
              half-increments
              readonly
              size="14"
            ></v-rating>

            <div class="grey--text ms-4">
              4.5 (413)
            </div>
          </v-row>

          <div class="my-4 text-subtitle-1">
            $ • Italian, Cafe
          </div>

          <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
        </v-card-text>

        <v-divider class="mx-4"></v-divider>

        <v-card-title>Tonight's availability</v-card-title>

      </v-card>
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
  data: () => ({
    topImage: require('@/assets/img/Bulbs_bar_counter.jpg'),
    philosophyImage: require('@/assets/img/bg-sp.png'),
    worksImage1: require('@/assets/img/tap_question.png'),
    worksImage2: require('@/assets/img/kashikan.png'),
    worksImage3: require('@/assets/img/three_tasks.png'),
    image_src: require('@/assets/img/Bulbs_bar_counter.jpg'),
    loading: false,
    selection: 0,
  }),

  methods: {
    reserve () {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    },
  },
}
</script>

<style lang="scss" scoped>
.bg_1 {
  background-color: antiquewhite;
}

.bg_2 {
  background-color: rgb(252, 247, 208);
}

.bg_3 {
  background-color: burlywood;
}
</style>
