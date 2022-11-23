<template>
  <v-app>
    <v-app-bar absolute color="#02343F" elevate-on-scroll dense>
      <v-btn fab height="45px" width="45px" icon>
        <v-icon>mdi-home-heart</v-icon>
      </v-btn>
      <v-tolbar-title>Please Sign Please</v-tolbar-title>
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
    <v-footer :absolute="!fixed">
      <span>Copyright 2022. doodoong all rights reserved.</span>
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
