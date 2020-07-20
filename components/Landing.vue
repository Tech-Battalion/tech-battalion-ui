<template>
    <div id="about">
      
      <v-container
            id="about-header"
            fluid
            class="teal lighten-2"
        >

            <v-row>
                <v-col>
                </v-col>
                <v-col>
                    <v-img
                        :src="require('../assets/axes-white.png')"
                        width="500"
                        height="300"
                    ></v-img>
                </v-col>
            </v-row>

        </v-container>

    </div>
</template>

<script>
export default {
    name: 'landing'
}
</script>

<style scoped>
    h1 {
        color: white;
    }
    p {
        color: white;
    }
</style>