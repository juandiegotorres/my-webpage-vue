<template>
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
          <li class="nav-item  px-4">
            <a href="" class="nav-link nav__a text-white">Sobre Mí</a>
          </li>
          <li class="nav-item  px-3">
            <a href="" class="nav-link nav__a text-white">Productos</a>
          </li>
          <li class="nav-item  px-3">
            <a href="" class="nav-link nav__a text-white">Proyectos</a>
          </li>
          <li class="nav-item  px-3">
            <a href="" class="nav-link nav__a text-white">Contacto</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
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
