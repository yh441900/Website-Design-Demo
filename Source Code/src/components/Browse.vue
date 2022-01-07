<template>
  <v-container fluid>
    <v-btn elevation="3" fab dark fixed bottom right color="indigo">
      <v-icon>mdi-help</v-icon>
    </v-btn>
    <v-row>
      <v-col cols="12">
        <v-carousel
          height="300"
          hide-delimiter-background
          :show-arrows="false"
          delimiter-icon="mdi-minus"
        >
          <!-- <v-carousel-item>
            <v-img
              src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
            />
          </v-carousel-item> -->

          <v-carousel-item>
            <v-sheet color="orange" height="100%" tile>
              <v-row class="fill-height" align="center" justify="center">
                <div class="text-h2">Advertisement 1</div>
              </v-row>
            </v-sheet>
          </v-carousel-item>

          <v-carousel-item>
            <v-sheet color="green" height="100%" tile>
              <v-row class="fill-height" align="center" justify="center">
                <div class="text-h2">Advertisement 2</div>
              </v-row>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
      </v-col>
    </v-row>
    <v-row></v-row>

    <v-row>
      <v-col>
        <v-tabs>
          <v-tab> 来自本地卖家 </v-tab>
          <v-tab> 来自国际卖家 </v-tab>
        </v-tabs>
      </v-col>
      <v-col align="right">
        <v-btn href="" target="_blank" text height="100%">
          <v-icon>mdi-filter-variant</v-icon>
          <div class="text-body-2">&nbsp;筛选排序</div>
        </v-btn>
        <v-btn href="" target="_blank" text height="100%">
          <v-icon>mdi-view-grid</v-icon>
          <div class="text-body-2">&nbsp;视图</div>
        </v-btn>
      </v-col>
    </v-row>

    <v-row class="text-center">
      <v-col v-for="n in 8" :key="n" cols="3">
        <v-card elevation="10" height="200"></v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-col></v-col>
    </v-row>
    <v-row>
      <v-col></v-col>
    </v-row>

    <v-row>
      <v-col cols="12">
        <v-footer>
          <v-card
            flat
            tile
            color="rgb(255, 0, 0, 0)"
            class="text-center"
            width="100%"
          >
            <v-card-text>
              <v-btn class="mx-4" text>
                <div class="text-body-2"><strong>国际买家注意事项</strong></div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">使用条款</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">帮助</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">隐私声明</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">联系我们</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">关于我们</div>
              </v-btn>
            </v-card-text>
            <v-card-text class="pt-0">
              UK's Largest Trading Place for New & Used Telescopes and
              Accessories<br />
              - Marking astronomy more affordable since 2003 -
            </v-card-text>

            <v-divider></v-divider>

            <v-card-text class="">
              © 2003 - {{ new Date().getFullYear() }}
              <strong>UK Astronomy Buy & Sell</strong>
            </v-card-text>
          </v-card>
        </v-footer>
      </v-col>
    </v-row>
  </v-container>
</template>
