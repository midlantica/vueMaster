<script setup>
  import { ref } from "vue";

  const product = ref([
    "Boots", "Hips", "Flips", "Chicks"
  ])

</script>

<template>
  <!-- <div class="flexRow gap1"> -->
    <aside>
      <nav>
        <ul>
          <li class="marBH" v-for="item in product"><a href="#">{{item}}</a></li>
        </ul>
      </nav>
    </aside>
    <div class="content">
      <div>
        <h2>Lorem ipsum dolor sit</h2>
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
        <div class="flexRow just-flex-end">
          <button role="button" class="">Submit</button>
        </div>

      </form>
    </div>
  <!-- </div> -->
</template>

<style lang="scss" scoped>
  aside {
    // position: sticky;

    ul {
      // margin: 0 !important;

      li {
        //

        a {
          font-weight: 600;
        }
      }
    }

  }

  .content {
    width: calc(100% - 13rem);
    // margin-left: 13rem;
    margin-right: 2rem;
    align-self: flex-end;
  }

</style>
