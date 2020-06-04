<template>
    <div>
      <v-footer color="red lighten-2" >
        <v-spacer></v-spacer>
        <div>&copy; {{ new Date().getFullYear() }}</div>
      </v-footer>
    </div>
</template>

<script>
    export default {
        name: 'Footer'
    }
</script>

<style lang="scss" scoped>

</style>