<template>
  <nav class="navbar navbar-expand-md bg-light navbar-light fixed-top">
    <a class="navbar-brand" href="javascript:void(0)" id="themeSwitchBtn">
      <img src="dist/images/avatar.jpeg" width="30px" height="30px" class="img-fluid rounded-circle" alt="">
      Jeric Epon
    </a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarsExampleDefault" aria-controls="navbarsExampleDefault" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarsExampleDefault">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item" v-for="(item, index) in 5" :key="index">
          <a class="nav-link" href="#">item {{index}} <span class="sr-only" v-if="index == 0">(current)</span></a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
  export default {
    name: 'Nav'
  }
</script>