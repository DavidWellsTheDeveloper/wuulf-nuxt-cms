<script setup></script>

<template>
  <section class="hero is-link is-medium is-bold">
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title is-size-1">
          <slot />
        </h1>
        <h2 class="subtitle mt-5">
            <slot name="subtitle"/>
        </h2>
      </div>
    </div>
  </section>
</template>

<style>
.hero-body {
  background-position: center;
  background-size: cover;
  background-repeat: no-repeat;
  height: 400px;
}
</style>