<template>
  <v-app>
    <v-app-bar app absolute color="#02343F" elevate-on-scroll dense>
      <nuxt-link to="/test">
        <v-btn fab height="45px" width="45px" icon>
          <v-icon>mdi-home-heart</v-icon>
        </v-btn>
      </nuxt-link>
      <v-tolbar-title class="text-yellow-50">Please Sign Please</v-tolbar-title>
      <v-spacer></v-spacer>
      <v-dialog transition="dialog-top-transition" max-width="600">
        <template #activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <v-icon>mdi-information-outline</v-icon>
          </v-btn>
        </template>
        <template #default="dialog">
          <v-card>
            <v-toolbar class="bg-green-700"> How to use </v-toolbar>
            <v-card-text>
              <div class="text-xl pa-12">This is how to use</div>
            </v-card-text>
            <v-card-actions class="justify-end">
              <v-btn text @click="dialog.value = false"> I understand </v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>
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
<style scoped>
.v-application {
  background-color: white;
}
</style>
