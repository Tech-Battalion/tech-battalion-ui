<template>
    <div id="discussion-board">
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
                    Discussion
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
                    Site | Twitter | Redit | Quora
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
    name: 'discussion-board'
}
</script>

<style scoped></style>