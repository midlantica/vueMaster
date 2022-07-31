<script setup>
  import { ref } from "vue";
  const product = ref("Boots")

</script>

<template>
  <div class="product-display">
    <div class="flexRow gap1">
      <div class="w30">
        <h1 class="mar0">{{product}}</h1>
      </div>
      <div class="">

        <form>

          <!-- Grid -->
          <div class="grid">

            <!-- Markup example 1: input is inside label -->
            <label for="firstname">
              First name
              <input type="text" id="firstname" name="firstname" placeholder="First name" required>
            </label>

            <label for="lastname">
              Last name
              <input type="text" id="lastname" name="lastname" placeholder="Last name" required>
            </label>

          </div>

          <!-- Markup example 2: input is after label -->
          <label for="email">Email address</label>
          <input type="email" id="email" name="email" placeholder="Email address" required>
          <small>We'll never share your email with anyone else.</small>

          <!-- Button -->
          <button type="submit">Submit</button>

        </form>

        <article>
          <header>Header</header>
          Body
          <footer>Footer</footer>
        </article>

        <div>
          <h3>Lorem ipsum dolor sit</h3>
          <p>amet consectetur adipisicing elit. Nobis quae animi quod facere ex delectus libero eius quasi distinctio, praesentium, incidunt et accusamus neque magni aliquam quam necessitatibus? Fugit, maxime?</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
