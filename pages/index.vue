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

    <v-col id="representative" class="bg_1 pa-16" cols="12">
      <div>
        <h1 class="indigo--text text--darken-4 text-h4 font-weight-bold mb-4">
          代表挨拶
        </h1>
      </div>
      <v-row justify="center" align="center">
        <v-col cols="12">
          <transition>
            <v-card
              v-show="representativeShow"
              class="scroll mx-auto my-12 translateY"
              max-width="500"
            >

              <v-img
                height="400"
                :src="representativeImage"
              ></v-img>

              <div class="text-left mx-4 mt-2">代表社員</div>
              <v-card-title class="test pt-0">鬼頭 訓志<span class="text-caption mx-2">KUNSHI KITO</span></v-card-title>

              <v-divider class="mx-4"></v-divider>

              <v-card-subtitle class="text-left">
                テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト

                テストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
                テキストテキスキストテキストテキストテキストテキストテキスト
                テキストテキストテキトテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
              </v-card-subtitle>

            </v-card>
          </transition>

        </v-col>
      </v-row>
    </v-col>

    <v-col id="news" class="bg_2 pa-16" cols="12">
      <div>
        <h1 class="indigo--text text--darken-4 text-h4 font-weight-bold mb-4">
          BLOG & NEWS
        </h1>
      </div>
      <div class="mb-6">
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
        テキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキストテキスト
      </div>

      <v-row justify="center" align="center">

        <v-col v-for="(blog, index) in blogs" :key="index" cols="12" md="4">
          <v-card height="400">
            <v-img
              height="220"
              :src="blog.imageUrl"
            ></v-img>

            <v-divider class="mx-4"></v-divider>

            <v-card-subtitle class="indigo--text text--darken-4">{{ textCut(blog.title, 14) }}</v-card-subtitle>

            <v-card-text>
              <div class="text-left">
                {{ textCut(blog.detail, 48) }}
              </div>
            </v-card-text>

          </v-card>
        </v-col>

      </v-row>
    </v-col>
    <v-col id="target" class="">
      <nuxt-link v-scroll-to="'#top'" to class="mr-2">トップへ</nuxt-link>
    </v-col>
  </v-row>
</template>

<script>
import { gsap } from "gsap";
import { ScrollTrigger } from 'gsap/ScrollTrigger'

if (process.client) {
  gsap.registerPlugin(ScrollTrigger)
}

export default {
  name: 'index',
  data () {
    return {
      topImage: require('@/assets/img/Bulbs_bar_counter.jpg'),
      philosophyImage: require('@/assets/img/bg-sp.png'),
      worksImage1: require('@/assets/img/tap_question.png'),
      worksImage2: require('@/assets/img/kashikan.png'),
      worksImage3: require('@/assets/img/three_tasks.png'),
      representativeImage: require('@/assets/img/me1.jpeg'),
      representativeShow: true,
      blogs: [
        {
          title: 'ブログ1',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/blog-image1.jpg'),
        },
        {
          title: 'ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2ブログ2',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/blog-image2.jpg'),
        },
        {
          title: 'ブログ3',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/blog-image1.jpg'),
        },
        {
          title: 'ブログ4',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/kashikan.png'),
        },
        {
          title: 'ブログ5',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/blog-image2.jpg'),
        },
        {
          title: 'ブログ6',
          detail: 'ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。ブログ本文。',
          imageUrl: require('@/assets/img/three_tasks.png'),
        },
      ],
    }
  },
  computed: {
  },
  methods: {
    textCut(text, max_length) {
      if(text.length > max_length){
        return text.substr(0, max_length) + '...'
      }
      return text
    },
    scrollItem() {
      gsap.fromTo('.scroll', {
        autoAlpha: 0,
        },
        {
          autoAlpha: 1,
          y: 0,
          duration: 2,
          scrollTrigger: {
            trigger: '.scroll',
            start: 'center center',
            markers: false
          }
        }
      )
    },
  },
  mounted() {
    this.scrollItem()
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

.translateY {
    transform: translateY(200px);
}
</style>
