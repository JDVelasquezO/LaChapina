<template>
    <div>
    <v-parallax
        v-if="this.$props.title == 'banner'"
        dark
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
      >
        <v-row
          align="center"
          justify="center"
        >
          <v-col class="text-center" cols="12">
            <v-img
              :src="require('../assets/logo.jpeg')"
              class="my-3"
              contain
              height="300"
            />
            <h1 class="display-1 font-weight-thin mb-4">{{ title }}</h1>
            <h4 class="subheading">Build your application today!</h4>
          </v-col>
        </v-row>
    </v-parallax>

    <v-parallax
        v-else-if="this.$props.title == 'carrousell'"
        dark
        src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
      >
        <v-row
          align="center"
          justify="center"
        >
          <v-col class="text-center" cols="8">
              <v-carousel hide-delimiters height="400">
                <v-carousel-item
                  v-for="(item,i) in items"
                  :key="i"
                  :src="item.src"
                ></v-carousel-item>
              </v-carousel>
          </v-col>
        </v-row>
    </v-parallax>
  </div>
</template>

<script>
    export default {
        name: 'Parallax',
        props: ['title'],
        data() {
          return {
            items: [
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
              },
              {
                src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
              },
            ],
          }
        },
    }
</script>

<style lang="scss" scoped>

</style>