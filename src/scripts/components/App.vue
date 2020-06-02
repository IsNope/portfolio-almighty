<template>
  <main class="px-0">
    <Nav />
    <div class="wrapper h-100">
      <HeroBanner />
      <Feature />
      <SkillSet />
      <Portfolio />
      <Interests />
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