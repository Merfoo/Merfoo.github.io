<template>
  <div>
    <nav class="navbar is-light is-spaced" role="navigation" aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <h1 class="title">
            <a class="navbar-item" href="/">
              FAUZI KLIMAN
            </a>
          </h1>

          <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbar">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>
        <div id="navbar" class="navbar-menu">
          <div class="navbar-end">
            <a class="navbar-item" href="/Fauzi_Kliman_Resume.pdf">
              Resume
            </a>
            <a class="navbar-item" href="https://www.linkedin.com/in/fauzikliman/">
              LinkedIn
            </a>
            <a class="navbar-item" href="https://github.com/Merfoo">
              GitHub
            </a>
          </div>
        </div>
      </div>
    </nav>
    <main class="main">
      <nuxt />
    </main>
    <footer class="footer">
      <div class="content has-text-centered">
        <div class="container">
          <p>
            Copyright © 2019 Fauzi Kliman
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

<script>
export default {
  mounted: function () {
    const $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0);
 
    if ($navbarBurgers.length > 0) {
      $navbarBurgers.forEach(el => {
        el.addEventListener('click', () => {
          const target = el.dataset.target;
          const $target = document.getElementById(target);

          el.classList.toggle('is-active');
          $target.classList.toggle('is-active');
        });
      });
    }
  }
}
</script>

<style>
</style>
