<template>
  <v-app>
    <v-container class="mt-5" >
      <v-layout justify-center>
        <v-flex xs10 md8 lg6>
          <v-img src="../assets/AdamYusufCropped.png"  class="mt-5"></v-img>
        </v-flex>
      </v-layout>
      <br>
      <v-layout justify-center>
        <v-flex xs8 md6>
          <h1 class="text-center">Hi, my name is <u>Adam Yusuf</u></h1>
        </v-flex>
      </v-layout>
      <br>
      <v-layout justify-center>
        <v-flex xs12 md6>
          <h1 class="text-center">I am an electrical engineering graduate with a passsion for making things work.</h1>
        </v-flex>
      </v-layout>
      </v-container>
      <v-container>
      <v-layout row wrap justify-center class="my-2">
        <v-flex xs6 sm3 md3 lg2 class="text-center my-2">
          <v-btn @click="goToResume()">See my resume</v-btn>
        </v-flex>
        <v-flex xs6 sm3 md3 lg2 class=" text-center my-2 ">
          <v-btn @click="goToProjects()">See my projects</v-btn>
        </v-flex>
        <v-flex xs6 sm3 md3 lg2 class="text-center my-2 ">
          <v-btn @click="goToAbout()">Learn about me</v-btn>
        </v-flex>
      </v-layout>
    </v-container>
    <v-footerr></v-footerr>
  </v-app>
</template>

<script>
export default {
  methods: {
    goToResume() {
      this.$router.push({ name: "resume" });
    },

    goToProjects() {
      this.$router.push({ name: "projects" });
    },

    goToAbout() {
      this.$router.push({ name: "about" });
    }
  }
};
</script>
