<template>
  <div class="home">
    <v-container>
    <img alt="Logo" src="https://image.freepik.com/free-vector/web-development-programmer-engineering-coding-website-augmented-reality-interface-screens-developer-project-engineer-programming-software-application-design-cartoon-illustration_107791-3863.jpg">
  
    <h2>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eius deserunt, modi ab velit delectus impedit. Tenetur cum libero natus. Nostrum nobis quisquam</h2>

    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita cumque aperiam maxime aliquam, amet animi molestias laboriosam rerum corporis, minima laudantium autem temporibus sint harum consequatur tempore. Aut, recusandae laboriosam.</p>
    </v-container>


    <v-footer
    dark
    padless
  >
    <v-card
      class="flex"
      flat
      tile
    >
      <v-card-title class="teal">
        <strong class="subheading">Get connected with us on social networks!</strong>

        <v-spacer></v-spacer>

        <v-btn
          v-for="icon in icons"
          :key="icon"
          class="mx-4"
          dark
          icon
        >
          <v-icon size="24px">
            {{ icon }}
          </v-icon>
        </v-btn>
      </v-card-title>

      <v-card-text class="py-2 white--text text-center">
        {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
      </v-card-text>
    </v-card>
  </v-footer>

  </div>
</template>

<script>
// @ is an alias to /src


export default {
  name: 'Home',
  data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  
}
</script>
