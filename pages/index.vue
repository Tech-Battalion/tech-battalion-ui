<template>
  <v-app id="inspire">

    <podcast-carousel />

    <header-bar />

    <nav-drawer-front />

    <v-content>
      
        <news-feed />
        
        <discussion-board />

        <support-portal />

        <cash-consult /> 
        
    </v-content>

    <footer-bar />

  </v-app>
</template>

<script>
import PodcastCarousel from '@/components/PodcastCarousel.vue';
import HeaderBar from '@/components/HeaderBar.vue';
import NavDrawerFront from '@/components/NavDrawerFront.vue';
import NewsFeed from '@/components/NewsFeed.vue';
import DiscussionBoard from '@/components/DiscussionBoard.vue';
import SupportPortal from '@/components/SupportPortal.vue';
import CashConsult from '@/components/CashConsult.vue';
import FooterBar from '@/components/FooterBar.vue';

export default {
  name: 'App',

  components: {
    PodcastCarousel,
    HeaderBar,
    NavDrawerFront,
    NewsFeed,
    DiscussionBoard,
    SupportPortal,
    CashConsult,
    FooterBar
  }
};
</script>