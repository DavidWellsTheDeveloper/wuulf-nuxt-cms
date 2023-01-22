<template>
  <NuxtLink :to="blogPost._path">
    <section class="blog-post-card card article">
      <div class="media">
        <figure v-if="blogPost.image" class="media-left ml-5">
          <p class="image is-128x128 is-square">
            <img
              class="is-rounded"
              style="border: 5px solid green"
              :src="blogPost.image"
              alt=""
            />
          </p>
        </figure>
        <div class="media-content has-text-centered">
          <h3 class="title article-title has-text-weight-bold">
            {{ blogPost.title }}
          </h3>
          <BlogPostMeta :author="blogPost.author" :date="blogPost.date" />
        </div>
      </div>
      <div class="card-content">
        <div class="content article-body is-size-5">
          {{ blogPost.description }}
        </div>
      </div>
    </section>
  </NuxtLink>
</template>

<script setup>
const props = defineProps({
  blogPost: {
    required: true
  },
});
</script>

<style lang="scss" scoped>
@media screen and (max-width: 500px) {
  .is-128x128 {
    max-width: 80px;
    max-height: 80px;
    margin-right: 0;
  }
}
</style>