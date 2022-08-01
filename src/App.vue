<script setup>
import ProductDisplay from './components/ProductDisplay.vue';
import Switch from './components/Switch.vue';
</script>

<template>
  <div class="container">
    <Switch />
    <header>
      <h1>VueMaster</h1>
    </header>
    <main>
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
    height: 57%;
  }

  aside {
    flex-basis: 30%;
    min-width: 120px;
  }

  footer {
    bottom: 1rem;
    height: 3rem;
  }
</style>
