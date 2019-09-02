<template>
  <div>
    <nav class="navbar is-spaced" role="navigation" aria-label="main navigation">
      <div class="container">
        <div class="navbar-brand">
          <h1 class="title">
            <a class="navbar-item" href="/">
              Fauzi Kliman
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
            <a class="navbar-item" href="/Fauzi_Kliman_Resume.pdf" target="_blank">
              Resume
            </a>
            <a class="navbar-item" href="https://www.linkedin.com/in/fauzikliman/" target="_blank">
              LinkedIn
            </a>
            <a class="navbar-item" href="https://github.com/Merfoo" target="_blank">
              GitHub
            </a>
          </div>
        </div>
      </div>
    </nav>
    <nuxt />
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
