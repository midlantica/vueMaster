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
  $green: hsl(150deg 76% 26%);
  $blue: hsl(200, 100%, 50%);

  header, footer {
    padding: 0.5rem 1.5rem;
    // color: whitesmoke;
    background: var(--primary);
    border-radius: 10px;
  }

  header {
    //
  }
  main {
    padding: 1rem 0;
    flex-grow: 1;
  }

  aside {
    flex-basis: 30%;
    min-width: 120px;
  }

  footer {
    //
  }

  // header, footer {
  //   background: $green;
  //   background: -moz-linear-gradient(0deg, $green 20%, $blue 100%);
  //   background: -webkit-linear-gradient(0deg, $green 20%, $blue 100%);
  //   background: linear-gradient(0deg, $green 20%, $blue 100%);
  // }
</style>
