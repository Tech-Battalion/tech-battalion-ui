<template>
    <div id="header-bar">
        <v-app-bar
        app
        clipped-left
        color="teal"
        >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />

        <v-img
            class="mx-2"
            :src="require('../assets/tech-battalion-logo.png')"
            max-height="80"
            max-width="300"
            contain
        ></v-img>

            <v-tabs
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
            
            </v-tabs>

        </v-app-bar>
    </div>
</template>

<script>
  export default {
    name: 'header-bar',
  }
</script>

<style scoped></style>