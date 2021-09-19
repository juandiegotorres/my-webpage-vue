<template>
  <!-- <div>
    <b-navbar toggleable="md" type="dark" variant="faded" fixed="top" id="nav">
      <div class="container">
        <h2 class="logo text-white">JTDev</h2>
        <button
          class="navbar-toggler"
          data-bs-target="#navbarNav"
          data-bs-toggle="collapse"
          aria-controls="navbarNav"
          aria-expanded="false"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse " id="navbarNav">
          <div class="mx-auto"></div>
          <ul class="navbar-nav text-white">
            <li class="nav-item px-4">
              <a href="" class="nav-link text-white">Sobre Mí</a>
            </li>
            <li class="nav-item px-3">
              <a href="" class="nav-link text-white">Productos</a>
            </li>
            <li class="nav-item px-3">
              <a href="" class="nav-link text-white">Proyectos</a>
            </li>
            <li class="nav-item px-3">
              <a href="" class="nav-link text-white">Contacto</a>
            </li>
          </ul>
        </div>
      </div>
    </b-navbar>
  </div> -->
  <div class="navbar navbar-expand-lg fixed-top" id="nav">
    <div class="container">
      <h2 class="logo text-white">JTDev</h2>
      <button
        class="navbar-toggler"
        data-bs-target="#navbarNav"
        data-bs-toggle="collapse"
        aria-controls="navbarNav"
        aria-expanded="false"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse " id="navbarNav">
        <div class="mx-auto"></div>
        <ul class="navbar-nav text-white">
          <li class="nav-item px-4">
            <a href="" class="nav-link text-white">Sobre Mí</a>
          </li>
          <li class="nav-item px-3">
            <a href="" class="nav-link text-white">Productos</a>
          </li>
          <li class="nav-item px-3">
            <a href="" class="nav-link text-white">Proyectos</a>
          </li>
          <li class="nav-item px-3">
            <a href="" class="nav-link text-white">Contacto</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
  <!-- <header class="navbar fixed-top navbar-expand-lg navba-dark p-md-3">
    <h2 class="logo">JTDev</h2>
    <nav>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a href="" class="nav-link text-black">Sobre mí</a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-link text-black">Productos</a>
          </li>
          <li class="nav-item">
            <a href="" class="nav-link text-black">Proyectos</a>
          </li>
        </ul>
      </div>
    </nav>
    <b-button variant="primary" class="boton">Contacto</b-button>
  </header> -->
</template>

<script>
export default {
  name: "HeaderComponent",
  mounted() {
    this.$nextTick(function() {
      window.addEventListener("scroll", function() {
        var navbar = document.getElementById("nav");
        var nav_classes = navbar.classList;
        if (document.documentElement.scrollTop >= 400) {
          if (nav_classes.contains("nav-solid") === false) {
            nav_classes.toggle("nav-solid");
          }
        } else {
          if (nav_classes.contains("nav-solid") === true) {
            nav_classes.toggle("nav-solid");
          }
        }
      });
    });
  },
};
</script>
