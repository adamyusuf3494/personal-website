<template>
  <v-app>
    <v-container class="mx-0 my-5" >
      <v-layout row wrap justify-center>
        <v-flex xs12 sm12 md12  lg2>
          <h2>Skills</h2>
        </v-flex>
        <v-flex xs12 sm12 md12 lg6>
          <ul>
                        <li>Proficient in <strong>HTML5</strong>, <strong>CSS3</strong>, <strong>JavaScript</strong>, <strong>JQuery</strong>, <strong>Php</strong>, <strong>MySQL</strong> and <strong>sass</strong></li>
                        <br>
                        <li>Experience with <strong>frameworks</strong> and <strong>bootstrap</strong></li>
                        <br>
                        <li>Competent in <strong>C++</strong>, <strong>Java</strong>, and <strong>C</strong></li>
                        <br>
                        <li>Comfortable with version control using<strong>git hub</strong></li>
                        <br>
                        <li>Experience using <strong>Jira</strong> and <strong>Confluence</strong> in a agile development</li>
                        <br>
                        <li>Extensive experience developing in <strong>Linux</strong>-based environments at various work placements</li>
                        <br>
                        <li>Familiar with common <strong>networking technologies</strong> and protocols</li>
                    </ul>
        </v-flex>
      </v-layout>
      <br>
      <br>
      <v-layout row wrap justify-center>
        <v-flex xs12 sm12 md12  lg2>
          <h2>Experience</h2>
        </v-flex>
        <v-flex xs12 sm12 md12  lg6>
            <h4><strong>Integration, Quality Assurance</strong> | Kinaxis | Sept 2018 - Aug 2019</h4>
          <ul>
              <li>Created test classes using <strong>Java</strong></li>
                        <br>
                        <li>Created and implemented test strategies to verify the product met acceptance criteria</li>
                        <br>
                        <li>Automated tests using Java to verify a variety of product feature which including, robustness, endurance to stress and boundary condition</li>
                        <br>
                        <li>Improved and refactored old test by using clean code (by Robert C. Martin) practices to reduce test flakiness and simplify the codebase</li>
          </ul>
        </v-flex>
      </v-layout>
      <br>
      <br>
      <v-layout row wrap justify-center>
        <v-flex xs12 sm12 md12  lg2>
          <h2>Projects</h2>
        </v-flex>
        <v-flex xs12 sm12 md12  lg6>
          <h4><strong>Snakes Board Game</strong> |  Jan 2020</h4>
                    <ul>
                        <li>Created a web bases snake game using vue framework</li>
                        <br>
                        <li>Implemented Firebase for authentication and leader board traking</li>
                        <br>
                        <li>Deployed game on my personal website</li>
                        <br>
                        <li>Stored <a href="https://github.com/adamyusuf3494/snakegamevue.git" target="_blank">source code</a> on git hub for version control</li>
                    </ul>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
export default {
    Skills:[
        {
            text:'Home',
            route:'/'
        },
        {
            text:'Resume',
            route:'/resume'
        },
        {
            text:'Projects',
            route:'/projects'
        },
        {
            text:'About',
            route:'/About'
        }
    ],
    Experience:[
        {
            icons: 'home',
            text:'Home',
            route:'/'
        },
        {
            icons: 'work',
            text:'Resume',
            route:'/resume'
        },
        {
            icons: 'assignment',
            text:'Projects',
            route:'/projects'
        },
        {
            icons: 'account_circle',
            text:'About',
            route:'/About'
        }
    ],
    Projects:[
        {
            icons: 'home',
            text:'Home',
            route:'/'
        },
        {
            icons: 'work',
            text:'Resume',
            route:'/resume'
        },
        {
            icons: 'assignment',
            text:'Projects',
            route:'/projects'
        },
        {
            icons: 'account_circle',
            text:'About',
            route:'/About'
        }
    ]
};
</script>

<style lang="scss" scoped>
</style>