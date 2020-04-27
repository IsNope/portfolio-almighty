<template lang="xml">
  <div class="hamburger" :class="{active: active}" @click="toggle()">
    <div class="line start"></div>
    <div class="line middle"></div>
    <div class="line end"></div>
  </div>
</template>
<script>
  export default {
    name: "HamburgerIcon",
    data() {
      return {
        active: false
      };
    },
    methods: {
      toggle() {
        this.active = !this.active;
      }
    }
  };
</script>