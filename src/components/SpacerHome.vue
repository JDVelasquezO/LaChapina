<template>
    <div>
      <v-container v-if='this.$props.info == "info1"'>
        <v-row class="text-center">
          <v-col cols="12">
          </v-col>

          <v-col class="mb-4">
            <h1 class="display-2 font-weight-bold mb-3">
              Welcome to Vuetify
            </h1>

            <p class="subheading font-weight-regular">
              For help and collaboration with other Vuetify developers,
              <br>please join our online
              <a
                href="https://community.vuetifyjs.com"
                target="_blank"
              >Discord Community</a>
            </p>
          </v-col>

          <v-col
            class="mb-5"
            cols="12"
          >
            <h2 class="headline font-weight-bold mb-3">
              What's next?
            </h2>

            <v-row justify="center">
              <a
                v-for="(next, i) in whatsNext"
                :key="i"
                :href="next.href"
                class="subheading mx-3"
                target="_blank"
              >
                {{ next.text }}
              </a>
            </v-row>
          </v-col>
        </v-row>
      </v-container>

      <v-container v-else-if="this.$props.info == 'info2'">
        <v-row class="text-center">
          <v-col cols="12">
          </v-col>

          <v-col class="mb-4">
            <h1 class="display-2 font-weight-bold mb-3">
              Welcome to Vuetify
            </h1>
          </v-col>
        </v-row>
      </v-container>
    </div>
</template>

<script>
    export default {
        name: 'SpacerHome',
        props: ['info'],
        data() {
            return {
                whatsNext: [
                    {
                    text: 'Explore components',
                    href: 'https://vuetifyjs.com/components/api-explorer',
                    },
                    {
                    text: 'Select a layout',
                    href: 'https://vuetifyjs.com/layout/pre-defined',
                    },
                    {
                    text: 'Frequently Asked Questions',
                    href: 'https://vuetifyjs.com/getting-started/frequently-asked-questions',
                    },
                ],
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>