<script setup>
  import { ref } from "vue";
const product = ref([
  "Boots", "Hips", "Flips", "Chicks"
])
const data = {
  objectItems: {
    key1: 'item1',
    key2: 'item2',
    key3: 'item3'
  },
  shoppingItems: [
    { name: 'apple', price: '7' },
    { name: 'orange', price: '12' }
  ]
}


</script>

<template>
  <div class="product-display">
    <div class="flexRow gap1">
      <aside>
        <nav>
          <ul>
            <li v-for="item in product"><a href="#">{{item}}</a></li>
          </ul>
        </nav>
      </aside>
      <div class="padR1">

        <div>
          <hgroup>
            <h2>Lorem ipsum dolor sit</h2>
            <h3>Lorem ipsum dolor sit</h3>
          </hgroup>
          <p>amet consectetur adipisicing elit. Nobis quae animi quod facere ex delectus libero eius quasi distinctio, praesentium, incidunt et accusamus neque magni aliquam quam necessitatibus? Fugit, maxime?</p>
        </div>

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


      </div>
    </div>
  </div>
</template>

<style scoped>

</style>
