<template>
  <div>
    <nav class="container">
      <h1>QuoteMaster</h1>
      <button id="navbar-button" @click="showNavbar">
        <span></span>
        <span></span>
        <span></span>
      </button>
      <ul>
        <li>
          <a target="_blank" href="https://awesome-stoicism.netlify.app">Awesome Stoicism Quotes</a>
        </li>
        <li>
          <a target="_blank" href="mailto:freeunioncoder@gmail.com">Questions?</a>
        </li>
        <li>
          <a target="_blank" href="https://github.com/uvacoder">More Projects</a>
        </li>
      </ul>
    </nav>
    <ul class="responsive-nav" :class="navbarVisible ? 'responsive-nav-active' : ''">
      <li>
          <a target="_blank" href="https://awesome-stoicism.netlify.app">Awesome Stoicism Quotes</a>
        </li>
      <li>
        <a target="_blank" href="mailto:freeunioncoder@gmail.com">Questions?</a>
      </li>
      <li>
        <a target="_blank" href="https://github.com/uvacoder">More Projects</a>
      </li>
    </ul>
    <header class="container-2">
      <p>
        QuoteMaster is a small website made by
        <a class="link" href="https://github/uvacoder/">Alec</a> for you to find quotes from well known individuals around the world.
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
