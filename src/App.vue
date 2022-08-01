<script setup>
import ProductDisplay from './components/ProductDisplay.vue';
import Switch from './components/Switch.vue';
</script>

<template>
  <div class="container">
    <header>
      <Switch />
      <h1>VueMaster</h1>
    </header>
    <main class="flexRow gap1">
      <ProductDisplay />
    </main>
    <footer>
      <h6>footer</h6>
    </footer>
  </div>
</template>

<style lang="scss">
  header, footer {
    padding: 0.5rem 1.5rem;
    color: var(--primary-inverse);
    background: var(--primary);
    border-radius: 10px;
    position: sticky;
    z-index: 10;
    width: 100%;
    max-width: 1280px;
    margin: 0 auto;
  }

  header {
    top: 1rem;
    height: 5rem;

  }
  main {
    margin: 2rem 0 2rem;
    overflow-y: auto;
    height: 70vh;
    // position: relative;
    // width: calc(100% - 13rem);
    // margin-left: 13rem;
    // margin-right: 2rem;
    padding-right: 2rem;
    // align-self: flex-end;
  }

  aside {
    // flex-basis: 30%;
    min-width: 200px;
    // position: fixed;
    // display: flex;
    // flex-direction: column;


    nav {
      position: fixed;
      display: flex;
      flex-direction: column;

    }
  }

  footer {
    bottom: 1rem;
    height: 3rem;
  }

  nav ol:last-of-type, nav ul:last-of-type {
    margin-right: calc(var(--nav-element-spacing-horizontal) * 0);
  }

  nav ol:first-of-type, nav ul:first-of-type {
      margin-left: calc(var(--nav-element-spacing-horizontal) * 0);
  }
</style>
