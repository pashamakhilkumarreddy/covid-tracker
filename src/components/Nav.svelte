<script>
export let segment;

let isNavBurgerOpen = false;
</script>

<header class="header">
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="/">
        <img src="https://bulma.io/images/bulma-logo.png" loading="lazy" decoding="async" importance="high" alt="Logo" />
      </a>

      <span role="button" class="navbar-burger burger" class:is-active={isNavBurgerOpen} aria-label="menu"
      aria-expanded="false" data-target="main-navbar" on:click={e => { isNavBurgerOpen = !isNavBurgerOpen } }>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </span>
    </div>

    <div id="main-navbar" class="navbar-menu" class:is-active={isNavBurgerOpen}>
      <div class="navbar-start">
        <a href="/" class="navbar-item" class:is-active={segment == undefined}>
          Home
        </a>

        <a href="/about" class="navbar-item" class:is-active={segment === 'about'}>
          About
        </a>
      </div>
    </div>
  </nav>
</header>

<style>
.header {
  border-bottom: 1px solid #ddd;
  box-shadow: 0 0 0.4rem 0 rgba(0, 0, 0, 0.3);
}
</style>