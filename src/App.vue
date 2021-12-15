<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <Contenido></Contenido>
    <SobreMi id="sobre-mi"></SobreMi>
    <Skills id="skills"></Skills>
    <Proyectos id="proyectos"></Proyectos>
    <Contacto id="contacto"></Contacto>
    <Footer></Footer>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import Contenido from "./components/Contenido.vue";
import SobreMi from "./components/SobreMi.vue";
import Skills from "./components/Skills.vue";
import Proyectos from "./components/Proyectos.vue";
import Contacto from "./components/Contacto.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    Contenido,
    SobreMi,
    Skills,
    Proyectos,
    Contacto,
    Footer,
  },
};
</script>

<style>
/* @import "./assets/css/w3.css"; */
@import "./assets/css/data.css";
@import "./assets/css/bootstrap-grid.css";
@import "./assets/css/styles.css";
@import "./assets/css/normalize.min.css";
@import "./assets/css/responsive.css";
</style>
