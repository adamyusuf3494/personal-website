<template>
  <v-app>
    <v-container class="pa-5">
      <v-layout row wrap justify-center class="px-5">
        <v-flex xs8 sm8 md8 lg2>
          <v-img alt="Vue logo" src="../assets/snakeProject.png" width="200px" />
        </v-flex>
        <v-flex xs8 sm8 md8 lg6 class="px-5">
          <p class="text-center">
            This project is a snake game that I build using vue framework. I incorporated firebase authentication to
            access the game. Firebase was also used to implement a backend to record the users score and to create a leaderboard
            <br />
            <strong>To use this project please log in</strong>
          </p>
          <v-btn class="text-xs-center">
            <a href="https://github.com/adamyusuf3494/snakegamevue.git" target="_blank">source code</a>
          </v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>