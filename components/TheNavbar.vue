<script setup>
const isMobileNavOpen = ref(false)
</script>

<template>
  <nav class="navbar">
    <div class="container">
      <div class="navbar-brand">
        <nuxt-link to="/wuulf2023" class="navbar-item has-text-weight-bold is-size-5">
          WUULF 2023
        </nuxt-link>
      </div>
      <div class="navbar-brand">
        <nuxt-link to="/" class="navbar-item has-text-weight-bold is-size-5">
          About WUULF
        </nuxt-link>
      </div>
    </div>
  </nav>
</template>

<style>
.navbar-brand {
  text-decoration: blue underline;
  margin-right: 10px;
}
</style>