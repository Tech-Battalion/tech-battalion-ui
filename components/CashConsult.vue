<template>
    <div id="cash-consult">
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
                    Consult
                </v-card-title>
                </v-card>
            </v-col>
            </v-row>

            <v-row no-gutters>
            <template v-for="n in 3">
                <v-col :key="n">
                <v-card
                    class="pa-2"
                    outlined
                    tile
                >
                    Live chat | Video call | Email | 
                </v-card>
                </v-col>
                <v-responsive
                v-if="n === 3"
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
    name: 'cash-consult'
}
</script>

<style scoped></style>