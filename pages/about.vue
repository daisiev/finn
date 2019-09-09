<template>
  <v-container class="text-center">
    <h1>About Me</h1>
    <v-row>
      <v-col cols="6">
        <v-img
          src="/profile.jpg"
          width="500px"
          position="center"
        >
        </v-img>
      </v-col>
      <v-col cols="6">
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eum porro animi soluta molestias odit nemo natus dolore enim eligendi. Officia veritatis accusantium repudiandae nam est quaerat ratione saepe! Ipsum eum aliquid quasi aperiam, maxime eos blanditiis eligendi ullam modi incidunt corporis magni sunt, deleniti numquam ut molestias, earum adipisci error esse quia. Eos expedita dignissimos ipsum? Eveniet tempora explicabo corporis molestias! Doloribus non rerum sapiente praesentium a aliquid ducimus omnis explicabo quibusdam nobis, quo sequi aspernatur et mollitia voluptatum fugit officiis ipsa quam placeat, similique eos aut. Ad repudiandae tempora id, labore, quod sed recusandae eos magni ullam similique magnam, et a amet accusamus deserunt nobis consequatur laborum ut quo! Est, sequi? In aut aliquid dicta corrupti. Quidem libero quas cupiditate itaque exercitationem incidunt ipsam veniam eveniet nobis suscipit vel placeat illum unde eum aut quae quos dicta nisi, omnis corporis aperiam sequi distinctio? Pariatur ipsum porro culpa sint amet cum officiis eos at iure excepturi illo deserunt tempora aliquid delectus, itaque autem modi repellendus unde quasi, impedit provident aliquam! A architecto minima, impedit ipsa sequi suscipit voluptatibus, voluptatem corrupti nihil mollitia molestias nisi! Alias, officia praesentium commodi, mollitia earum repellendus accusamus ullam quod nulla, enim delectus voluptas accusantium. Id.</p>
      </v-col>
    </v-row>

    <nuxt-link to="/contact">
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
    <nuxt-link to="/">
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
