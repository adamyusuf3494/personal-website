<template>
  <v-app>
    <v-container class="hidden-md-and-down">
      <v-layout row wrap justify-center class="my-2">
        <v-flex lg1.5 xl1 class="text-center my-2">
          <v-btn class="primary" @click="goToHome()">Home</v-btn>
        </v-flex>
        <v-flex lg1.5 xl1 class="text-center my-2">
          <v-btn class="primary" @click="goToResume()">Resume</v-btn>
        </v-flex>
        <v-flex lg1.5 xl1 class="text-center my-2">
          <v-btn class="primary" @click="goToProjects()">Projects</v-btn>
        </v-flex>
        <v-flex lg1.5 xl1 class="text-center my-2">
          <v-btn class="primary" @click="goToAbout()">About</v-btn>
        </v-flex>
      </v-layout>
    </v-container>

    <v-toolbar class="hidden-lg-and-up">
      <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </v-toolbar>

    <v-navigation-drawer v-model="drawer" app class="hidden-lg-and-up primary">
      <v-list color="transparent">
        <v-list-item v-for="link in links" :key="link.text" router :to="link.route">
          <v-list-item-action>
            <v-icon class="white--text">{{link.icons}}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title class="white--text pa-3">{{link.text}}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      links: [
        {
          icons: "home",
          text: "Home",
          route: "/"
        },
        {
          icons: "work",
          text: "Resume",
          route: "/resume"
        },
        {
          icons: "assignment",
          text: "Projects",
          route: "/projects"
        },
        {
          icons: "account_circle",
          text: "About",
          route: "/About"
        }
      ]
    };
  },
  methods: {
    goToHome() {
      this.$router.push({ name: "home" });
    },

    goToResume() {
      this.$router.push({ name: "resume" });
    },

    goToProjects() {
      this.$router.push({ name: "projects" });
    },

    goToAbout() {
      this.$router.push({ name: "about" });
    }
  },
  watch: {
    $route: {
      handler: function(route) {
        route;
      },
      deep: true,
      immediate: true
    }
  }
};
</script>

<style lang="scss" scoped>
</style>