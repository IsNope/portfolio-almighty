<template>
  <section class="portfolio">
    <div class="container portfolio-title">
      <div class="h1 text-center">Portfolio</div>
    </div>
    <div class="row container mx-auto p-0" id="grid">
      <a
        href="#"
        target="_blank"
        class="col-lg-4 col-md-6 col-sm-6 col-6 p-0 portfolio-item"
        v-for="i in 6"
        :key="i"
      >
        <figure class="m-0">
          <img :src="`dist/images/temp/project/${i}.png`" alt srcset />
          <div class="portfolio-item-overlay d-flex justify-content-center align-items-center">
            <div class="title">
              <span>Portfolio {{ i }}</span>
            </div>
          </div>
        </figure>
      </a>
    </div>
  </section>
</template>

<script>
// require("slick-carousel");
export default {
  mounted() {
    // $("#grid").slick({
    //   arrows: false,
    // });
  }
};
</script>
