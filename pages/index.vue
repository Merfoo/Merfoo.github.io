<template>
    <div>
      <section class="section">
        <div class="container has-text-centered">
          <p>
            Hello, I am a graduate from Oregon State University (March 2020) with a Bachelor of Science in Computer Science.
          </p>
          <p>
            I like to write software in C++, Python 3, JavaScript, C#, and C for people to use and enjoy!
          </p>
          <p>
            <a href="/Fauzi_Kliman_Resume.pdf">Resume</a> |
            <a href="https://www.linkedin.com/in/fauzikliman/">LinkedIn</a> |
            <a href="https://github.com/Merfoo">GitHub</a>
          </p>
        </div>
      </section>
      <section class="section">
        <div class="container has-text-centered projects">
          <ProjectCard class="project-card">
            <template v-slot:image>
              <a href="https://merfoo-notes.netlify.com/">
                <img src="~assets/notes.png"/>
              </a>
            </template>
            <template v-slot:content>
              <h1 class="title is-5">
                Notes
              </h1>
              <p>Make an account or login to create public or private notes!</p>
              <a href="https://merfoo-notes.netlify.com/">[Live]</a>
              <a href="https://github.com/Merfoo/notes">[GitHub]</a>
            </template>
          </ProjectCard>

          <ProjectCard class="project-card">
            <template v-slot:image>
              <a href="https://merfoo.github.io/fsm/">
                <img src="~assets/fsm.png"/>
              </a>
            </template>
            <template v-slot:content>
              <h1 class="title is-5">
                Finite State Machine
              </h1>
              <p>Create finite state machine diagrams that you can download and share with others!</p>
              <a href="https://merfoo.github.io/fsm/">[Live]</a>
              <a href="https://github.com/Merfoo/fsm">[GitHub]</a>
            </template>
          </ProjectCard>

          <ProjectCard class="project-card">
            <template v-slot:image>
              <a href="https://merfoo.github.io/Breakout/">
                <img src="~assets/breakout.png"/>
              </a>
            </template>
            <template v-slot:content>
              <h1 class="title is-5">
                Breakout
              </h1>
              <p>The classic Breakout game with the ability to create custom levels and download a picture of the level!</p>
              <a href="https://merfoo.github.io/Breakout/">[Live]</a>
              <a href="https://github.com/Merfoo/Breakout">[GitHub]</a>
            </template>
          </ProjectCard>

          <ProjectCard class="project-card">
            <template v-slot:image>
              <a href="https://merfoo.github.io/Asteroidz/">
                <img src="~assets/asteroids.png"/>
              </a>
            </template>
            <template v-slot:content>
              <h1 class="title is-5">
                Asteroids
              </h1>
              <p>Traverse through procedurally generated asteroids coming at you from all directions with only movement and lazer attacks to assist you!</p>
              <a href="https://merfoo.github.io/Asteroidz/">[Live]</a>
              <a href="https://github.com/Merfoo/Asteroidz">[GitHub]</a>
            </template>
          </ProjectCard>

          <ProjectCard class="project-card">
            <template v-slot:image>
              <a href="https://merfoo.github.io/Epileptic-Snake-Game/">
                <img src="~assets/snake.png"/>
              </a>
            </template>
            <template v-slot:content>
              <h1 class="title is-5">
                Snake
              </h1>
              <p>A crazy colorful snake game featuring multiple game modes that you can play with friends!</p>
              <a href="https://merfoo.github.io/Epileptic-Snake-Game/">[Live]</a>
              <a href="https://github.com/Merfoo/Epileptic-Snake-Game">[GitHub]</a>
            </template>
          </ProjectCard>
        </div>
      </section>
    </div>
</template>

<script>
import ProjectCard from '~/components/ProjectCard.vue';

export default {
  components: {
    ProjectCard
  }
}
</script>

<style scoped>
.project-card {
  margin: 10px;
  width: 600px;
}

.projects {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>
