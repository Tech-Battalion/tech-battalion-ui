<template>
    <div id="news-feed">

        <v-container
            id="news-header"
            fluid
        >
            <v-row>
                <v-col>
                </v-col>
                <v-col>
                    <h1 class="text-center">News</h1>
                </v-col>
                <v-col>
                </v-col>
            </v-row>

        </v-container>

        <v-container
            fluid
            id="news-body"
        >

            <v-row
                v-for="i in 1"
                :key="i"
            >
                <v-col
                    v-for="j in 3"
                    :key="j"
                >
                    <v-card class="d-inline-block mx-auto" :elevation=10>

                        <v-container>

                            <v-card-text class="headline font-weight-bold">
                                <!-- {{ normalizedNewsData[i].title }} -->
                                Man Shot and Survived by Heroically Swinging like Spiderman
                            </v-card-text>

                            <v-row justify="space-between">
                            <v-col cols="auto">
                                <v-img
                                height="220"
                                width="220"
                                :src="require('../assets/MC_DotModus.jpg')"
                                ></v-img>
                            </v-col>
                    
                            <v-col
                                cols="auto"
                                class="text-center pl-0"
                            >
                                <v-row
                                class="flex-column ma-0 fill-height"
                                justify="center"
                                >
                                <v-col class="px-0">
                                    <v-btn icon>
                                    <v-icon>mdi-heart</v-icon>
                                    </v-btn>
                                </v-col>
                    
                                <v-col class="px-0">
                                    <v-btn icon>
                                    <v-icon>mdi-bookmark</v-icon>
                                    </v-btn>
                                </v-col>
                    
                                <v-col class="px-0">
                                    <v-btn icon>
                                    <v-icon>mdi-share-variant</v-icon>
                                    </v-btn>
                                </v-col>
                                </v-row>
                            </v-col>
                            </v-row>
                        </v-container>
                    </v-card>
                    
                </v-col>
            </v-row>
        </v-container>
    </div>
    
</template>

<script>
    export default {
        name: 'news-feed',
        props: {
            newsData: Object,
        },
        computed: {
            normalizedNewsData: function () {
                return this.newsData.items
            }
        }
    }
</script>

<style scoped></style>