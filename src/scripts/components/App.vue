<template>
  <main class="px-0">
    <Nav />
    <div class="wrapper h-100">
      <HeroBanner />
      <Feature />
      <SkillSet />
      <!-- <Portfolio /> -->
      <MiniProjects />
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
  },
  mounted() {
    fetch("data/data.json").then(data => data.json() ).then(result => console.log(result))
  }
};
</script>