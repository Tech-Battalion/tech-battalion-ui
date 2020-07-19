<template>
    <div id="header-bar">
        <v-navigation-drawer
            v-model="drawerRight"
            app
            clipped
            right
            color="blue-grey lighten-1"
        >
        <v-list> 
          <v-list-item @click.stop="right = !right">
            <v-spacer></v-spacer>
            <v-list-item-action>
              <v-img
                :src="require('../assets/news-logo.png')"
                width="90"
                heigh="18"
              ></v-img>
            </v-list-item-action>
            <v-list-item-content>
            </v-list-item-content>
          </v-list-item>

          <v-list-item @click.stop="right = !right">
            <v-spacer></v-spacer>
            <v-list-item-action>
              <v-img
                :src="require('../assets/about-logo.png')"
                width="100"
                heigh="20"
              ></v-img>
            </v-list-item-action>
            <v-list-item-content>
            </v-list-item-content>
          </v-list-item>

          <v-list-item @click.stop="right = !right">
            <v-spacer></v-spacer>
            <v-list-item-action>
              <v-img
                :src="require('../assets/contact-logo.png')"
                width="125"
                heigh="25"
              ></v-img>
            </v-list-item-action>
            <v-list-item-content>
            </v-list-item-content>
          </v-list-item>
        </v-list>
        </v-navigation-drawer>

        <v-app-bar
            app
            clipped-right
            color="blue-grey lighten-1"
            dark
            elevation="0"
        >
            <v-img
                class="mx-2"
                :src="require('../assets/tech-battalion-logo.png')"
                max-height="80"
                max-width="300"
                contain
            ></v-img>
            <v-spacer></v-spacer>
            <v-app-bar-nav-icon 
                @click.stop="drawerRight = !drawerRight" 
            ></v-app-bar-nav-icon>
        </v-app-bar>

        <!-- <v-navigation-drawer
            v-model="drawer"
            app
            clipped
            color="blue-grey"
            temporary
            class='mt-5'
            style='top: 45px'
            overlay-color="blue-grey"
        >

            <v-list dense>
                <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-podcast</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Podcast</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
                <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-forum</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Discussion</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
                <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-newspaper-variant-multiple-outline</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Tech News</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
                <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-google-cloud</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Cloud Support</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
            <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-cash-multiple</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Consult</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
            <v-list-item link>
                <v-list-item-action>
                    <v-icon>mdi-comment-quote</v-icon>
                </v-list-item-action>
                <v-list-item-content>
                    <v-list-item-title>Feedback</v-list-item-title>
                </v-list-item-content>
                </v-list-item>
            </v-list>
        </v-navigation-drawer> -->

    </div>
</template>

<script>
  export default {
    name: 'header-bar',
    name: 'drawerRight', 
    data () {
      return {
        drawerRight: null
      }
    }
  }
</script>

<style scoped></style>