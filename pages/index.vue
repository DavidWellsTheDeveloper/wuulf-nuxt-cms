<template>
    <main>
      <TheHero>
        About WUULF
        <template v-slot:subtitle>WUULF (Western Unitarian Universalist Life Festival) is a 
            week-long, multi-generational camp for Unitarian-Universalists from 
            June 19th-June 25th, 2023 at the Ghost Ranch in New Mexico. We are a loving 
            community from a diverse set of age groups, backgrounds, and cultures who gather 
            in New Mexico each year to express our appreciation for each other and our world.</template>
      </TheHero>
      <WUULFGeneralList />
    </main>
  </template>
  
  <script>
    export default {
      name: "About WUULF"
    }
  </script>
  
  <style lang="scss" scoped>
  
  </style>