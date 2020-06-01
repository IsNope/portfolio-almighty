<template>
  <section class="portfolio">
    <div class="container portfolio-title">
      <div class="h1 text-center">Portfolio</div>
    </div>
    <div class="row portfolio container mx-auto p-0" id="grid">
      <div class="col col-lg-4 col-md-6 p-0" v-for="i in 6" :key="i">
        <figure class="m-0">
          <img :src="`dist/images/temp/project/${i}.png`" alt srcset />
        </figure>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  mounted: () => {
    let Masonry = require("masonry-layout");

    var msnry = new Masonry("#grid", {
      // options...
    });
  }
};
</script>

<style>
</style>