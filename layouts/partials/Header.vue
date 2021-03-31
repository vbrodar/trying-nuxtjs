<template>
  <header>
    <h3 class="logo">Nuxt Website</h3>
    <ul>
      <li>
        <nuxt-link to="/">Home</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/about">About</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/contact">Contact</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/donate">Donate</nuxt-link>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
@use "../../assets/main.scss";
</style>
