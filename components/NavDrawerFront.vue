<template>
    <div id="nav-drawer-front">
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
    name: 'nav-drawer-front'
}
</script>

<style scoped></style>