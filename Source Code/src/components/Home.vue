<template>
  <v-container fluid>
    <v-btn
      elevation="3"
      fab
      dark
      fixed
      bottom
      right
      color="indigo"
    >
      <v-icon>mdi-help</v-icon>
    </v-btn>
    <v-row>
      <v-col cols="12">
        <v-carousel
          height="400"
          hide-delimiter-background
          :show-arrows="false"
          delimiter-icon="mdi-minus"
        >
          <v-carousel-item>
            <v-img
              src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
            />
          </v-carousel-item>

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
      <v-col cols="9">
        <v-tabs>
          <v-tab>
            <v-icon>mdi-star</v-icon>
            &nbsp;Featured Advertisement
          </v-tab>
          <v-tab>
            <v-icon>mdi-history</v-icon>
            &nbsp;Recent Advertisements
          </v-tab>
          <v-tab>
            <v-icon>mdi-newspaper-variant-outline</v-icon>
            &nbsp;Product Reviews
          </v-tab>
        </v-tabs>
      </v-col>
      <v-col align="right">
        <v-btn href="" target="_blank" text height="100%">
          <v-icon>mdi-dots-horizontal</v-icon>
          <div class="text-body-2">&nbsp;Explore More</div>
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
          <v-card flat tile color="rgb(255, 0, 0, 0)" class="text-center" width="100%">
            <v-card-text>
              <v-btn class="mx-4" text>
                <div class="text-body-2">Terms of Use</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">Help</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">Privacy Statement</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">Contact US</div>
              </v-btn>
              <v-btn class="mx-4" text>
                <div class="text-body-2">About US</div>
              </v-btn>
            </v-card-text>
            <v-card-text class="pt-0">
              UK's Largest Trading Place for New & Used Telescopes and
              Accessories<br />
              - Marking astronomy more affordable since 2003 -
            </v-card-text>

            <v-divider></v-divider>

            <v-card-text class="">
              © 2003 - {{ new Date().getFullYear() }} <strong>UK Astronomy Buy & Sell</strong>
            </v-card-text>
          </v-card>
        </v-footer>
      </v-col>
    </v-row>
  </v-container>
</template>
