<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          class="my-3"
          contain
          height="200"
        />
      </v-col>
      <v-col cols="12">
        <v-text-field
          label="搜索"
          placeholder="键入搜索内容"
          solo
          clearable
          append-outer-icon="mdi-magnify"
        ></v-text-field>
      </v-col>
    </v-row>

    <v-row>
      <v-col class="d-flex justify-center">
        <v-checkbox label="允许国际卖家"></v-checkbox>
        <a
          >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</a
        >
        <v-checkbox label="显示无法送达的商品"></v-checkbox>
      </v-col>
    </v-row>

    <v-row><v-col></v-col></v-row>

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