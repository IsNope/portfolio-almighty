<template>
    <main class="px-0" :class="{dark}">
        <Nav/>
        <div class="wrapper">
            <Styleguide/>
        </div>
    </main>
</template>

<script>
    export default {
      name: 'App',
      data() {
          return {
            dark: false
          }
      },
        mounted() {
            console.log('Component mounted.')
        }
    }
</script>