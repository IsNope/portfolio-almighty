<template>
  <main class="px-0">
    <Nav />
    <div class="wrapper">
      <Styleguide />
    </div>
  </main>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      dark: false
    };
  }
};
</script>