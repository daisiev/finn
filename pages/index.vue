<template>
  <v-container class="text-center">
    <v-img
      src="/logo.png"
      alt=""
    ></v-img>
    <v-row>
      <v-col
        cols="6"
        v-for="image in images"
        v-bind:key="image"
      >
        <v-img :src="image">
        </v-img>
      </v-col>
    </v-row>
    <nuxt-link to="/about">
      <v-btn
        fixed
        dark
        fab
        bottom
        right
        outlined
        color="pink lighten-4"
      >
        <v-icon>mdi-chevron-right</v-icon>
      </v-btn>
    </nuxt-link>
    <nuxt-link to="/contact">
      <v-btn
        fixed
        dark
        fab
        bottom
        left
        outlined
        color="pink lighten-4"
      >
        <v-icon>mdi-chevron-left</v-icon>
      </v-btn>
    </nuxt-link>
  </v-container>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    Logo,
    VuetifyLogo
  },
  data: () => {
    return {
      images: [
        '/portfolio/1.jpg',
        '/portfolio/2.jpg',
        '/portfolio/3.jpg',
        '/portfolio/4.jpg',
        '/portfolio/5.jpg',
      ]
    }
  }
}
</script>
