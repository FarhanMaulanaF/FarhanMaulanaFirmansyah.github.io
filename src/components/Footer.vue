<template>
  <v-footer
    dark
    padless
  >
    <v-card
      flat
      tile
      class="black lighten-1 white--text text-center"
    >
      <v-card-text>
        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4 white--text"
          icon
        >
          <v-icon size="24px" >
              {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-text>

      <div>
        <a class="white--text" href="https://www.linkedin.com/in/farhan-maulana-firmansyah-530153159/" target="_blank" style="text-decoration: none">LinkedIn &nbsp;</a>
        <a class="white--text" href="https://www.Instagram.com/firmansyahmaa_/" target="_blank" style="text-decoration: none">Instagram</a>
      </div>

      <br/>

      <v-card-text class="white--text pt-0">
        Thank you sincerely for your kind visit. It meant a lot to me that you took the time to come by. I know how busy you are, and I truly value the time we spent together represents by this page. Please know that I am very grateful for your kindness.
        <br/>
        - Farhan Firmansyah -
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text>
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
      name: 'Footer',

    data: () => ({
      icons: [
          'mdi-linkedin', 
          'mdi-instagram',
      ],
    }),
  }
</script>