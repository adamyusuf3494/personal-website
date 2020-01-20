<template>
  <v-app>
    <Navbar v-show="$route.name !== 'home'" />

    <v-content>
      <router-view></router-view>
    </v-content>

    <v-footer>
      <v-row class="transparent darker-2 text-center black--text" justify="center" no-gutters>
        <v-btn
          v-for="icon in icons"
          :key="icon.name"
          color="white"
          text
          rounded
          class="primary mx-2 my-1"
        >
          <a :href="icon.link" :target="icon.target">
            <v-icon color="white">{{ icon.name }}</v-icon>
          </a>
        </v-btn>
        <v-col class="transparent darker-2 text-center black--text" cols="12">
          <span>
            &copy;2020 —
            <strong>Adam Yusuf</strong>
          </span>
        </v-col>
      </v-row>
    </v-footer>
  </v-app>
</template>

<script>
import Navbar from "@/components/Navbar";
import { mdiGithubBox, mdiLinkedin } from "@mdi/js";
export default {
  name: "App",
  components: { Navbar },

  data: () => ({
    icons: [
      {
        name: "email",
        link: "mailto:adamyusuf3494@gmail.com",
        target: "_blank"
      },
      {
        name: mdiGithubBox,
        link: "https://www.linkedin.com/in/adam-yusuf",
        target: "_blank"
      },
      {
        name: mdiLinkedin,
        link: "https://github.com/adamyusuf3494/",
        target: "_blank"
      }
    ]
  })
};
</script>
