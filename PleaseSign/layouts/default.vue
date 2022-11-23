<template>
  <v-app>
    <v-app-bar app absolute color="#02343F" elevate-on-scroll dense>
      <v-btn fab height="45px" width="45px" icon>
        <v-icon>mdi-home-heart</v-icon>
      </v-btn>
      <v-tolbar-title class="text-yellow-50">Please Sign Please</v-tolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-information-outline</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer :absolute="!fixed" color="#02343F">
      <span class="text-yellow-50"
        >Copyright 2022. doodoong all rights reserved.</span
      >
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {}
  },
}
</script>
