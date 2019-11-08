<template>
    <div class="container">
      <section class="section">
        <div class="container">
          <h1 class="title is-4">
            About
          </h1>
          <p>
            Hello, I am a soon to graduate (March 2020) from Oregon State University with a Bachelor of Science in Computer Science.
          </p>
          <p>
            I like to write software in C/C++, Python 3, and JavaScript for people to use and enjoy!
          </p>
          <p>
          </p>
        </div>
      </section>
      <section class="section">
        <div class="container">
          <h1 class="title is-4">
            Projects
          </h1>
          <div class="columns">
            <div class="column">
              <BulmaCard class="bulma-card">
                <template v-slot:image>
                  <a href="https://merfoo.github.io/fsm/">
                    <img src="~assets/fsm.png"/>
                  </a>
                </template>
                <template v-slot:content>
                  <h1 class="title is-5">
                    Finite State Machine
                  </h1>
                  <a href="https://merfoo.github.io/fsm/">[Live]</a>
                  <a href="https://github.com/Merfoo/fsm">[Source]</a>
                </template>
              </BulmaCard>

              <BulmaCard class="bulma-card">
                <template v-slot:image>
                  <a href="https://merfoo.github.io/Asteroidz/">
                    <img src="~assets/asteroids.png"/>
                  </a>
                </template>
                <template v-slot:content>
                  <h1 class="title is-5">
                    Asteroids
                  </h1>
                  <a href="https://merfoo.github.io/Asteroidz/">[Live]</a>
                  <a href="https://github.com/Merfoo/Asteroidz">[Source]</a>
                </template>
              </BulmaCard>
            </div>
            <div class="column">
              <BulmaCard class="bulma-card">
                <template v-slot:image>
                  <a href="https://merfoo.github.io/Breakout/">
                    <img src="~assets/breakout.png"/>
                  </a>
                </template>
                <template v-slot:content>
                  <h1 class="title is-5">
                    Breakout
                  </h1>
                  <a href="https://merfoo.github.io/Breakout/">[Live]</a>
                  <a href="https://github.com/Merfoo/Breakout">[Source]</a>
                </template>
              </BulmaCard>

              <BulmaCard class="bulma-card">
                <template v-slot:image>
                  <a href="https://merfoo.github.io/Epileptic-Snake-Game/">
                    <img src="~assets/snake.png"/>
                  </a>
                </template>
                <template v-slot:content>
                  <h1 class="title is-5">
                    Snake
                  </h1>
                  <a href="https://merfoo.github.io/Epileptic-Snake-Game/">[Live]</a>
                  <a href="https://github.com/Merfoo/Epileptic-Snake-Game">[Source]</a>
                </template>
              </BulmaCard>
            </div>
          </div>
        </div>
      </section>
    </div>
</template>

<script>
import BulmaCard from '~/components/BulmaCard.vue';

export default {
  components: {
    BulmaCard
  }
}
</script>

<style scoped>
.bulma-card {
  margin-top: 25px;
}
</style>
