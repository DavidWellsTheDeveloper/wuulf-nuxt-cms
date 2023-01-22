<template>
  <figure class="image is-128X128">
    <img :src="url" :alt="alt" />
  </figure>
</template>

<script setup>
const props = defineProps({
  url: {
    type: String,
    required: true,
  },
  alt: {
    type: String,
    required: false,
    default: ""
  }
});
</script>

<style>
.counter {
  max-width: 500px;
  padding: 15px;
  margin: 0 auto;
  border: 3px solid #ccc;
  text-align: center;
}

.counter .current-count {
  margin-bottom: 10px;
  text-align: center;
  font-size: 1.5rem;
}

.counter button {
  font-size: 1rem;
  padding: 5px;
}
</style>