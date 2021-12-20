<template>
  <nav id="nav-bar">
    <!-- <img :src="require('@/assets/images/logo.png')" class="logo-xl" alt /> -->
    <img
      :src="require('@/assets/images/logo_mobile.png')"
      class="logo-mobile"
      alt="logo"
      v-on:click="nav('inicio')"
    />
    <input type="checkbox" id="click" />
    <label class="menu-btn" id="submenu" v-on:click="ulActivo">
      <img src="https://icongr.am/entypo/menu.svg?size=40&color=ffffff" alt="submenu" />
    </label>
    <ul v-bind:class="{ 'ul__activo': estaActivo }" id="menu-mobile">
      <li>
        <a v-on:click="nav('sobre-mi')">Sobre Mí</a>
      </li>
      <li>
        <a class v-on:click="nav('skills')">Skills</a>
      </li>
      <li>
        <a v-on:click="nav('proyectos')">Proyectos</a>
      </li>
      <li>
        <a v-on:click="nav('contacto')">Contacto</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "HeaderComponent",
  data() {
    return {
      estaActivo: false,
    }
  },
  mounted() {
    this.$nextTick(function () {
      window.addEventListener("scroll", function () {
        var navbar = document.getElementById("nav-bar");
        var nav_classes = navbar.classList;
        if (document.documentElement.scrollTop >= 500) {
          if (nav_classes.contains("nav-solid") === false && nav_classes.contains("nav__sm") === false) {
            nav_classes.toggle("nav-solid");
            nav_classes.toggle("nav__sm");
          }
        } else {
          if (nav_classes.contains("nav-solid") === true && nav_classes.contains("nav__sm") === true) {
            nav_classes.toggle("nav-solid");
            nav_classes.toggle("nav__sm");
          }
        }
      });
    });
  },
  methods: {
    nav(link) {
      if (link == 'inicio') {
        position = 0;
      } else {
        //Obtengo la posicion de la seccion
        var position = document.getElementById(link).offsetTop;
        //Cierro el menu-mobile si esta desde el telefono
        this.estaActivo = false;
        //Le resto a la posicion para que encuadre en la pantalla
        position -= 92;
      }
      window.scrollTo({ top: position, behavior: "smooth" });
    },

    ulActivo() {
      this.estaActivo = !this.estaActivo;
    }
  }
};
</script>
