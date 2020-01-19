<template>
  <v-app>
    <footer />
      <Navbar v-show="$route.name !== 'home'"/>
      
    <v-content>
      <router-view></router-view>
    </v-content>
    
    <v-footer>
            <v-row
            class="transparent darker-2  text-center black--text"
        justify="center"
        no-gutters
      >
           <v-btn
          v-for="icon in icons"
          :key="icon"
          color="white"
          text
          rounded
          class=" primary mx-2 my-1"
        >
          <v-icon>{{ icon }}</v-icon>
          
        </v-btn> 
        <v-col
          class="transparent darker-2  text-center black--text"
          cols="12"
        >
          <span>&copy;2020 — <strong>Adam Yusuf</strong></span>
        </v-col>
            </v-row>
    </v-footer>
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar'
export default {
  name: 'App',
  components: { Navbar  },

  

  data: () => ({
    icons: [
      'email',
      'fab fa-linkedin',
      'fab fa-github'
    ],
  }),
};
</script>
