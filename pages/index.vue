<template>
    <main class="main">
      <div class="container">
        <div class="columns">
          <div class="column">
            <BulmaCard class="bulma-card">
              <template v-slot:image>
                <a href="https://merfoo.github.io/fsm/" target="_blank">
                  <img src="~assets/fsm.png"/>
                </a>
              </template>
              <template v-slot:content>
                <a href="https://github.com/Merfoo/fsm" target="_blank">
                  Finite State Machine (2017)
                </a>
              </template>
            </BulmaCard>

            <BulmaCard class="bulma-card">
              <template v-slot:image>
                <a href="http://merfoo.github.io/Asteroidz/" target="_blank">
                  <img src="~assets/asteroids.png"/>
                </a>
              </template>
              <template v-slot:content>
                <a href="https://github.com/Merfoo/Asteroidz" target="_blank">
                  Asteroids (2014)
                </a>
              </template>
            </BulmaCard>
          </div>
          <div class="column">
            <BulmaCard class="bulma-card">
              <template v-slot:image>
                <a href="http://merfoo.github.io/Breakout/" target="_blank">
                  <img src="~assets/breakout.png"/>
                </a>
              </template>
              <template v-slot:content>
                <a href="https://github.com/Merfoo/Breakout" target="_blank">
                  Breakout (2015)
                </a>
              </template>
            </BulmaCard>

            <BulmaCard class="bulma-card">
              <template v-slot:image>
                <a href="http://merfoo.github.io/Epileptic-Snake-Game/" target="_blank">
                  <img src="~assets/snake.png"/>
                </a>
              </template>
              <template v-slot:content>
                <a href="https://github.com/Merfoo/Epileptic-Snake-Game" target="_blank">
                  Snake (2013)
                </a>
              </template>
            </BulmaCard>
          </div>
        </div>
      </div>
    </main>
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
