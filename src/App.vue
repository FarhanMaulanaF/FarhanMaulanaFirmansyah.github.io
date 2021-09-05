<template>
  <v-app>
    <v-app-bar
      app
      color="black"
      dark
    >
      <div class="d-flex align-center">
        <h2>Personal Page</h2>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/FarhanMaulanaF"
        target="_blank"
        text
      >
        <span class="mr-2">github collection</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HelloWorld/>
      <br/>
      <Footer/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/Identity.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',

  components: {
    HelloWorld,
    Footer,
  },

  data: () => ({
  }),
};
</script>
