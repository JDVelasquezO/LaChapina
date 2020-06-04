<template>
  <div>
    <Parallax />
    <SpacerHome />
    <Parallax />
      <!-- <v-parallax
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
      </v-parallax> -->
      <SpacerHome />
        <!-- <v-container>
        <v-row class="text-center">
          <v-col cols="12">
          </v-col>

          <v-col class="mb-4">
            <h1 class="display-2 font-weight-bold mb-3">
              Welcome to Vuetify
            </h1>
          </v-col>
        </v-row>
      </v-container> -->
  </div>
</template>

<script>
  import Parallax from '@/components/Parallax';
  import SpacerHome from '@/components/SpacerHome';

  export default {
    name: 'HelloWorld',
    components: {
      Parallax,
      SpacerHome
    },
    data: () => ({
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
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
        {
          text: 'github',
          href: 'https://github.com/vuetifyjs/vuetify',
        },
        {
          text: 'awesome-vuetify',
          href: 'https://github.com/vuetifyjs/awesome-vuetify',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
        {
          text: 'Chat',
          href: 'https://community.vuetifyjs.com',
        },
        {
          text: 'Made with Vuetify',
          href: 'https://madewithvuejs.com/vuetify',
        },
        {
          text: 'Twitter',
          href: 'https://twitter.com/vuetifyjs',
        },
        {
          text: 'Articles',
          href: 'https://medium.com/vuetify',
        },
      ],
    }),
  }
</script>
