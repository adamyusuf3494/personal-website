<template>
  <div>
    <v-container class="pa-5 my-5">
      <v-layout row wrap justify-center class="px-5" >
        <v-flex xs10 sm10 md10 lg2 class="pa-5">
          <v-img alt="Vue logo" src="../assets/snakeProject.png" width="200px" />
        </v-flex>
        <v-flex xs10 sm10 md10 lg6 class="pa-5">
          <p >
            This project is a snake game that I build using vue framework. I incorporated firebase authentication to
            access the game. Firebase was also used to implement a backend to record the users score and to create a leaderboard
            <br />
            <strong>Note: To use this project please log in</strong>
          </p>
          <v-btn class=" primary" align-center>
            <a href="https://github.com/adamyusuf3494/snakegamevue.git" target="_blank"><span class=" white--text"> Source code</span></a>
          </v-btn>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
</style>