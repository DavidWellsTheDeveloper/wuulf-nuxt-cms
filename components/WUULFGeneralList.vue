<script setup>

const { data: wuulfgeneralinfo } = useAsyncData("wuulfgeneralinfo", () => {
  return queryContent("/wuulfgeneralinfo").sort({date: -1}).find();
});

// const postsSorted = reactive({
//   wuulfgeneralinfo: wuulfgeneralinfo.sortBy('date', 'asc')
// })
</script>

<template>
  <div class="container">
    <section class="articles">
      <div class="column is-8 is-offset-2">

        <div
          v-for="blogPost in wuulfgeneralinfo"
          :key="blogPost._path"
          class="card article"
        >
        <ListItem :blogPost="blogPost"></ListItem>
        </div>
      </div>
    </section>
  </div>
</template>

<style>
.blog-post-card {
  padding-top: 2.5rem;
  padding-bottom: 3rem;
}

.blog-post-card .card-content {
  padding: 1rem;
}

.blog-post-card .title {
  margin-bottom: 1rem;
}
</style>