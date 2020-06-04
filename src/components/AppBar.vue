<template>
    <div>
        <v-app-bar
        app
        color="red lighten-2"
        dark
        >
        <div class="d-flex align-center">
            <v-img
            alt="Vuetify Logo"
            class="shrink mr-2"
            contain
            src="../assets/logo.jpeg"
            transition="scale-transition"
            width="60"
            />
        </div>

        <v-spacer></v-spacer>

        <v-btn
            href="https://github.com/vuetifyjs/vuetify/releases/latest"
            target="_blank"
            text
        >
            <span class="mr-2">Latest Release</span>
            <v-icon>mdi-open-in-new</v-icon>
        </v-btn>
        </v-app-bar>
    </div>
</template>

<script>
    export default {
        name: 'AppBar'
    }
</script>

<style lang="scss" scoped>

</style>