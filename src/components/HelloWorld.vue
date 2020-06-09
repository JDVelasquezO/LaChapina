<template>
  <div>
    <Parallax title="banner" />
    <SpacerHome info="info2" />
    <Parallax title="carrousell" />
    <SpacerHome info="info1" />
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
