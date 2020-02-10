<template>
  <div class="site">
    <div class="container has-text-centered">
      <p class="title is-1 navbar-item">
        FAUZI KLIMAN
      </p>
    </div>
    <main class="main">
      <nuxt />
    </main>
    <footer class="footer">
      <div class="content">
        <div class="container has-text-centered">
          <p>
            Copyright © 2020 Fauzi Kliman
          </p>
          <a href="https://github.com/Merfoo">
            <img src="~assets/GitHub-Mark-32px.png"/>
          </a>
          <a href="https://www.linkedin.com/in/fauzikliman/">
            <img src="~assets/LinkedIn-Black-34px-R.png"/>
          </a>
        </div>
      </div>
    </footer>
  </div>
</template>

<style>
.site {
  display: flex;
  min-height: 100vh;
  flex-direction: column;
}

.main {
  flex: 1
}
</style>
