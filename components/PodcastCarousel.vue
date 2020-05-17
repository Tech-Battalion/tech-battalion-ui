<template>
    <div id="podcast-carousel">

        <v-carousel v-model="carousel">
            <v-carousel-item
            v-for="(item,i) in items"
            :key="i"
            :src="item.src"
            ></v-carousel-item>
        </v-carousel>

    </div>
</template>

<script>
  export default {
    name: 'podcast-carousel',
    data () {
      return {
        carousel: 0, 
        items: []
      }
    }
  };
  
</script>

<style scoped></style>

