<template>
  <v-container class="text-center">
    <v-img
      src="/logo.png"
      alt
    ></v-img>
    <v-row>
      <v-col
        :md="6"
        :sm="12"
        v-for="imageData in images"
        v-bind:key="imageData.image"
      >
        <v-img
          class="art-image"
          :src="imageData.image"
          @click="openDialog(imageData)"
        ></v-img>
        <v-dialog
          v-model="dialogOpen"
          max-width="800"
        >
          <v-card>
            <v-img
              class="white--text"
              :src="currentDialog.image"
              max-height="500"
            >
              <v-card-title class="align-end fill-height">{{ currentDialog.title }}</v-card-title>
            </v-img>
            <v-card-text>{{ currentDialog.description }}</v-card-text>
          </v-card>
        </v-dialog>
      </v-col>
    </v-row>
    <nuxt-link to="/about">
      <v-btn
        fixed
        dark
        fab
        top
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
        top
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
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  components: {
    Logo,
    VuetifyLogo
  },
  data: () => {
    return {
      images: [
        {
          image: "/portfolio/1.jpg",
          title: "Art Title",
          description: "Art Description"
        },
        {
          image: "/portfolio/2.jpg",
          title: "Art Title",
          description: "Art Description"
        },
        {
          image: "/portfolio/3.jpg",
          title: "Art Title",
          description: "Art Description"
        },
        {
          image: "/portfolio/4.jpg",
          title: "Art Title",
          description: "Art Description"
        },
        {
          image: "/portfolio/5.jpg",
          title: "Art Title",
          description: "Art Description"
        }
      ],
      currentDialog: {},
      dialogOpen: false
    };
  },
  methods: {
    openDialog(dialog) {
      this.currentDialog = dialog;
      this.dialogOpen = true;
    }
  }
};
</script>

<style scoped>
.art-image:hover {
  transition: 1000ms;
  cursor: pointer;
  filter: saturate(0);
}
</style>
