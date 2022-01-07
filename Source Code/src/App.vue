<template>
  <v-app>
    <v-app-bar color="indigo-darken-3" dark app clipped-left>
      <div class="d-flex align-center">
        <v-img
          alt="Vuetify Logo"
          class="shrink mr-2"
          contain
          src="https://cdn.vuetifyjs.com/images/logos/vuetify-logo-dark.png"
          transition="scale-transition"
          width="40"
        />
      </div>

      <v-spacer></v-spacer>

      <v-btn href="" target="_blank" text>
        <span class="mr-2">&nbsp;浏览商品</span>
      </v-btn>

      <v-btn href="" target="_blank" text>
        <span class="mr-2">&nbsp;商品信息存档</span>
      </v-btn>

      <v-btn href="" target="_blank" text>
        <!-- <v-icon>mdi-web</v-icon> -->
        <span class="mr-2">&nbsp;关于我们</span>
      </v-btn>

      <v-btn href="" target="_blank" text>
        <v-icon>mdi-magnify</v-icon>
        <!-- <span class="mr-2">&nbsp;Language</span> -->
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer permanent expand-on-hover app clipped dark>
      <v-list>
        <v-list-item class="px-2">
          <v-list-item-avatar>
            <v-img
              src="https://randomuser.me/api/portraits/women/2.jpg"
            ></v-img>
          </v-list-item-avatar>
        </v-list-item>
        <v-list-item link>
          <v-list-item-content>
            <v-list-item-title class="text-h6"> 李飞飞 </v-list-item-title>
            <v-list-item-subtitle>someone@somewhere.com</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </v-list>

      <v-divider></v-divider>

      <v-list nav dense>
        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-home</v-icon>
          </v-list-item-icon>
          <v-list-item-title style="font-weight: bold">主页</v-list-item-title>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-basket-check</v-icon>
          </v-list-item-icon>
          <v-list-item-title style="font-weight: bold">购买订单</v-list-item-title>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-advertisements</v-icon>
          </v-list-item-icon>
          <v-list-item-title style="font-weight: bold">上架商品</v-list-item-title>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-eye-check</v-icon>
          </v-list-item-icon>
          <v-list-item-title style="font-weight: bold">愿望清单</v-list-item-title>
        </v-list-item>

        <v-list-item link>
          <v-list-item-icon>
            <v-icon>mdi-bell-badge</v-icon>
          </v-list-item-icon>
          <v-list-item-title style="font-weight: bold">消息</v-list-item-title>
        </v-list-item>
      </v-list>

      <template v-slot:append>
        <v-list nav dense>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-ideogram-cjk</v-icon>
            </v-list-item-icon>
            <v-list-item-title style="font-weight: bold"
              >切換為正體</v-list-item-title
            >
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-web</v-icon>
            </v-list-item-icon>
            <v-list-item-title style="font-weight: bold"
              >语言</v-list-item-title
            >
          </v-list-item>
          <v-list-item link>
            <v-list-item-icon>
              <v-icon>mdi-logout-variant</v-icon>
            </v-list-item-icon>
            <v-list-item-title style="font-weight: bold"
              >注销</v-list-item-title
            >
          </v-list-item>
        </v-list>
      </template>
    </v-navigation-drawer>

    <v-main>
      <!-- <HelloWorld /> -->
      <!-- <homepage /> -->
      <browse />
      <!-- <search /> -->
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
// import homepage from "./components/Home.vue";
import browse from "./components/Browse.vue"
// import search from "./components/Search.vue"

export default {
  name: "App",

  components: {
    // HelloWorld,
    // homepage,
    browse,
    // search,
  },

  data: () => ({
    //
  }),
};
</script>
