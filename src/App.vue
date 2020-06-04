<template>
  <v-app>
    <AppBar />
    <v-content>
      <HelloWorld/>
    </v-content>
    <Footer />
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import AppBar from './components/AppBar';
import Footer from './components/Footer';

export default {
  name: 'App',

  components: {
    HelloWorld,
    AppBar,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
