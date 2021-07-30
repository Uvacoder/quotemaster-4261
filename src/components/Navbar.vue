<template>
  <div>
    <nav class="container">
      <h1>Quotify</h1>
      <button id="navbar-button" @click="showNavbar">
        <span></span>
        <span></span>
        <span></span>
      </button>
      <ul>
        <li>
          <a target="_blank" href="mailto:rsiyq924@gmail.com">Questions?</a>
        </li>
        <li>
          <a target="_blank" href="https://github.com/fu4303">More Projects</a>
        </li>
      </ul>
    </nav>
    <ul class="responsive-nav" :class="navbarVisible ? 'responsive-nav-active' : ''">
      <li>
        <a target="_blank" href="mailto:rsiyq924@gmail.com">Questions?</a>
      </li>
      <li>
        <a target="_blank" href="https://github.com/fu4303">More Projects</a>
      </li>
    </ul>
    <header class="container-2">
      <p>
        Quotify is a small website made by
        <a class="link" href="https://github/fu4303/">Alec</a> for you to find quotes from well known individuals around the world.
      </p>
      <p class="instructions">Just click on the quote and it will be copied to your clipboard.</p>
    </header>
  </div>
</template>

<script>
export default {
  data() {
    return {
      navbarVisible: true
    };
  },
  methods: {
    showNavbar() {
      this.navbarVisible = !this.navbarVisible;
    }
  }
};
</script>

<style>
</style>
