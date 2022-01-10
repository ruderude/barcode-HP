<template>
  <div>
    <v-footer
      color="indigo darken-4"
      dark
      app
      absolute
    >
      <v-container>
        <v-row class="pa-12">
          <v-col cols="2" md="1">
            <v-divider
              class="mx-4"
              color=""
              vertical
            ></v-divider>
          </v-col>
          <v-col cols="10" md="5">
            <div class="yellow--text text--accent-4">
              <span class="font-weight-bold">会社概要</span><br>
              BarCodeSystems合同会社<br>
              〒164-0003<br>
              東京都中野区東中野4丁目1-1英ビル2F<br>
              設立 : 2021年9月29日<br>
              代表社員 鬼頭 訓志<br>
              Email: hogehogehoge
            </div>
          </v-col>
          <v-col cols="2" md="1">
            <v-divider
              class="mx-4"
              color=""
              vertical
            ></v-divider>
          </v-col>
          <v-col cols="10" md="5">
            <div class="yellow--text text--accent-4">
              <span class="font-weight-bold">NEWS</span><br>

              2018.07.06ページ更新しました。<br>
              2018.07.06ページ更新しました。<br>
              2018.07.06ページ更新しました。<br>
              2018.07.06ページ更新しました。<br>
              2018.07.06ページ更新しました。<br>

            </div>
          </v-col>
        </v-row>

        <v-row justify="center" align="center">
          <v-col class="text-center">
            <span class="yellow--text text--accent-4">&copy; BarCodeSystems合同会社 All Rights Reserved.</span>
          </v-col>
        </v-row>
      </v-container>

    </v-footer>
  </div>
</template>

<script>
export default {
  name: 'footer_d',
  data () {
    return {
    }
  },
  methods: {
  },
  mounted () {
  }
}
</script>

<style>
</style>
