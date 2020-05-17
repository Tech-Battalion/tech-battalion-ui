<template>
    <div id="support-portal">
        <v-container
        class="fill-height"s
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
                    Cloud Support
                </v-card-title>
                </v-card>
            </v-col>
            </v-row>

            <v-row no-gutters>
            <template v-for="n in 4">
                <v-col :key="n">
                <v-card
                    class="pa-2"
                    outlined
                    tile
                >
                    Tutorials | Whitepapers | Key Notes | Docs
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
    name: 'support-portal'
}
</script>

<style scoped></style>