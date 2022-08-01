<script setup>
  const toggleTheme = () => {
    let targetTheme = "light"
    const currentTheme = document.documentElement.getAttribute("data-theme")
    if (currentTheme === "light") {
      targetTheme = "dark";
    }
    document.documentElement.setAttribute('data-theme', targetTheme)
    localStorage.setItem('theme', targetTheme)
  }
</script>

<template>
  <label class="switch">
    <input type="checkbox" @click="toggleTheme">
    <span class="slider round"></span>
  </label>
</template>

<style lang="scss" scoped>
  $width: 1rem;
  $height: $width;

  /* The switch - the box around the slider */
  .switch {
    position: absolute;
    display: inline-block;
    width: 1.7rem;
    height: $width;
    z-index: 100;
    top: 1rem;
    right: 1.25rem;
  }

  /* Hide default HTML checkbox */
  .switch input {
    opacity: 0;
    width: 0;
    height: 0;
  }

  /* The slider */
  .slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #ccc;
    -webkit-transition: .4s;
    transition: .4s;
  }

  .slider:before {
    position: absolute;
    content: "";
    height: $width;
    width: $width;
    left: 0px;
    bottom: 0px;
    background-color: white;
    -webkit-transition: .4s;
    transition: .4s;
  }

  input:checked + .slider {
    background-color: var(--teal-900);
  }

  input:focus + .slider {
    box-shadow: 0 0 1px var(--teal-900);
  }

  input:checked + .slider:before {
    -webkit-transform: translateX($width);
    -ms-transform: translateX($width);
    transform: translateX($width);
  }

  /* Rounded sliders */
  .slider.round {
    border-radius: $width;
  }

  .slider.round:before {
    border-radius: $width;
  }
</style>