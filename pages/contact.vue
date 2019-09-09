
<template>
  <v-container class="text-center">
    <h1>Contact Me!</h1>

    <v-card class="pa-8">
      <v-row class="pa-8">
        <v-col cols="6">
          <v-text-field label="Name"></v-text-field>
        </v-col>
        <v-col cols="6">
          <v-text-field label="Email"></v-text-field>
        </v-col>
        <v-col cols="12">
          <v-textarea label="Message">
          </v-textarea>
        </v-col>
      </v-row>
      <v-btn
        outlined
        color="pink lighten-4"
      >Submit</v-btn>
    </v-card>

    <nuxt-link to="/">
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
    <nuxt-link to="/about">
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
export default {

}
</script>
