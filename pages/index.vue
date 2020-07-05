<template>
  <v-app 
      id="inspire" 
      teal
  >
  <!-- :style="{background: $vuetify.theme.themes.dark.background}" -->

    <!-- <podcast-carousel /> -->

    <header-bar />

    <v-content>

        <news-feed :newsData=articleMeta />
        
        <!-- <discussion-board /> -->

        <support-portal />

        <about />

        <cash-consult /> 
        
    </v-content>

    <footer-bar />

  </v-app>
</template>

<script>
import axios from 'axios';

import PodcastCarousel from '@/components/PodcastCarousel.vue';
import HeaderBar from '@/components/HeaderBar.vue';
import About from '@/components/About.vue';
import NewsFeed from '@/components/NewsFeed.vue';
import DiscussionBoard from '@/components/DiscussionBoard.vue';
import SupportPortal from '@/components/SupportPortal.vue';
import CashConsult from '@/components/CashConsult.vue';
import FooterBar from '@/components/FooterBar.vue';

export default {
  name: 'App',
  async asyncData (context) {
            const { data } = await axios.get(`http://127.0.0.1:8000/api/v2/pages/`).catch(error => console.log(error));
            return { articleMeta: data }
  },

  components: {
    PodcastCarousel,
    HeaderBar,
    NewsFeed,
    About,
    DiscussionBoard,
    SupportPortal,
    CashConsult,
    FooterBar
  }
};
</script>