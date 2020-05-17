<template>
    <div id="news-feed">
        <v-container
        class="fill-height"
        >
            <v-row no-gutters>
            <v-col>
                <v-card
                class="pa-2"
                outlined
                tile
                >
                <v-card-title
                    class="justify-center"
                >
                    Tech News
                </v-card-title>
                </v-card>
            </v-col>
            </v-row>

            <v-row no-gutters>
            <template v-for="n in 8">
                <v-col :key="n">
                <v-card
                    class="pa-2"
                    outlined
                    tile
                >
                    Article 1, 2 , 3
                </v-card>
                </v-col>
                <v-responsive
                v-if="n === 4"
                :key="`width-${n}`"
                width="100%"
                ></v-responsive>
            </template>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'news-feed'
}
</script>

<style scoped></style>