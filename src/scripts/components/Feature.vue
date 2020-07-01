<template>
  <section class="feature">
    <div class="container">
      <div class="row">
        <div class="col-md-4 mb-lg-0 mb-sm-5 mb-5">
          <FeatherIcon class="feature-icon" />
          <div class="feature-title">Optimized Website</div>
          <p class="feature-body mx-lg-0">
            I always consider writing CLEAN & DRY code and proper testing to achieve a fast and light weight website.
          </p>
        </div>
        <div class="col-md-4 mb-lg-0 mb-sm-5 mb-5">
          <CodeIcon class="feature-icon" />
          <div class="feature-title">Pixel-Perfect</div>
          <p class="feature-body mx-lg-0">
            I love to translate design into a clean code without wasting any pixels and bringing it into a user friendly UI. 
          </p>

        </div>
        <div class="col-md-4 mb-lg-0 mb-sm-5 mb-0"> <!-- LAST CHILD -->
          <ResponsiveIcon class="feature-icon" />
          <div class="feature-title">Resposive & Mobile First</div>
          <p class="feature-body mx-lg-0">
            Due to years of experience, I gained a lot of skills including the ability to write a code that supports mobile and smaller devices.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'Feature'
  }
</script>