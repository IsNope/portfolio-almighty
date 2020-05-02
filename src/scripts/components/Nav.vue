<template>
  <nav class="navbar navbar-expand-md bg-light navbar-light fixed-top">
    <div class="container pr-lg-0">
      <a class="navbar-brand" href="javascript:void(0)">
        <img
          src="dist/images/avatar.jpeg"
          width="30px"
          height="30px"
          class="img-fluid rounded-circle"
          alt
        />
        <span>Jeric Epon</span>
      </a>
      <div class="d-md-none d-block">
        <HamburgerIcon />
      </div>

      <div class="collapse navbar-collapse" id="navbarsExampleDefault">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#">
              <InstagramIcon />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <FacebookIcon />
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">
              <LinkedinIcon />
            </a>
          </li>
          <li class="nav-item" @click="switchTheme()">
            <a
              class="nav-link"
              id="light-mode"
              href="javascript:void(0)"
              data-toggle="tooltip"
              data-placement="bottom"
              title="Join the dark side?"
            >
              <DarkIcon />
            </a>
            <a
              class="nav-link"
              id="dark-mode"
              href="javascript:void(0)"
              data-toggle="tooltip"
              data-placement="bottom"
              title="Comback to light!"
            >
              <LightIcon />
            </a>
          </li>
          <li class="nav-item">
            <a
              class="nav-link"
              href="#"
              data-toggle="tooltip"
              data-placement="bottom"
              title="Turn on/off the bugs"
            >
              <BugIcon />
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Nav",
  methods: {
    switchTheme() {
      document.body.classList.toggle("dark");
    }
  }
};
</script>