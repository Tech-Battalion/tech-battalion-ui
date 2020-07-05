<template>
    <div id="header-bar">
        <v-app-bar
        app
        clipped-left
        color="teal"
        >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

            <v-img
                class="mx-2"
                :src="require('../assets/tech-battalion-logo.png')"
                max-height="80"
                max-width="300"
                contain
            ></v-img>

            <!-- <v-tabs
                centered
            >
                <v-tab>Podcast
                <v-icon>mdi-podcast</v-icon>
                </v-tab>
                <v-divider
                class="mx-4"
                inset
                vertical
                ></v-divider>

                <v-tab>Discussion
                <v-icon>mdi-forum</v-icon>
                </v-tab>
                <v-divider
                class="mx-4"
                inset
                vertical
                ></v-divider>

                <v-tab>Tech News
                <v-icon>mdi-newspaper-variant-multiple-outline</v-icon>
                </v-tab>
                <v-divider
                class="mx-4"
                inset
                vertical
                ></v-divider>

                <v-tab>Cloud Support
                <v-icon>mdi-google-cloud</v-icon>
                </v-tab>
                <v-divider
                class="mx-4"
                inset
                vertical
                ></v-divider>

                <v-tab>Consult
                <v-icon>mdi-cash-multiple</v-icon>
                </v-tab>
                <v-divider
                class="mx-4"
                inset
                vertical
                ></v-divider>

                <v-tab>Feedback
                <v-icon>mdi-comment-quote</v-icon>
                </v-tab>
            
            </v-tabs> -->

        </v-app-bar>

        <v-navigation-drawer
            v-model="drawer"
            app
            clipped
            color="white"
            temporary
            class='mt-5'
            style='top: 46px'
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
        </v-navigation-drawer>

    </div>
</template>

<script>
  export default {
    name: 'header-bar',
    name: 'drawer',
    data () {
      return {
        drawer: 0, 
        items: []
      }
    }
  }
</script>

<style scoped></style>