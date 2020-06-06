<template>
    <div id="news-feed">

        <v-container
            class="fill-height"
        >
            <h1>News</h1>  

            <v-row
                v-for="i in 3"
                :key="i"
            >
                <v-col
                    v-for="j in 3"
                    :key="j"
                >
                    <v-card
                        class="mx-auto"
                        color="#26c6da"
                        dark
                        max-width="400"
                    >
                        <v-card-text class="headline font-weight-bold">
                            {{ normalizedNewsData[i].title }}
                        </v-card-text>
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