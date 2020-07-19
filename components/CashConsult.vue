<template>
    <div id="cash-consult">
        <v-container
            id="consult-header"
            fluid
            class="blue-grey lighten-1"
        >
            <v-row>
                <v-col>
                </v-col>
                <v-col>
                    <h1 class="text-center">Contact</h1>
                    <p> Fill out the form bitch. </p>
                    <p> Fill out the form bitch. </p>
                    <p> Fill out the form bitch. </p>
                    <p> Fill out the form bitch. </p>
                </v-col>
                <v-col>
                </v-col>
            </v-row>

        </v-container>

        <!-- <v-container
            class="blue-grey lighten-1"
        >
            <form>
                <v-text-field
                    v-model="name"
                    :error-messages="nameErrors"
                    :counter="10"
                    label="Name"
                    required
                    @input="$v.name.$touch()"
                    @blur="$v.name.$touch()"
                ></v-text-field>
                <v-text-field
                    v-model="email"
                    :error-messages="emailErrors"
                    label="E-mail"
                    required
                    @input="$v.email.$touch()"
                    @blur="$v.email.$touch()"
                ></v-text-field>
                <v-select
                    v-model="select"
                    :items="items"
                    :error-messages="selectErrors"
                    label="Item"
                    required
                    @change="$v.select.$touch()"
                    @blur="$v.select.$touch()"
                ></v-select>
                <v-checkbox
                    v-model="checkbox"
                    :error-messages="checkboxErrors"
                    label="Do you agree?"
                    required
                    @change="$v.checkbox.$touch()"
                    @blur="$v.checkbox.$touch()"
                ></v-checkbox>
            
                <v-btn class="mr-4" @click="submit">submit</v-btn>
                <v-btn @click="clear">clear</v-btn>
            </form>
        </v-container> -->

    </div>
</template>

<script>
    export default {
        name: 'cash-consult'
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