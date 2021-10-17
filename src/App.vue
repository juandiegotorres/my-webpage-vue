<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <Contenido></Contenido>
    <SobreMi></SobreMi>
    <Proyectos></Proyectos>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import Contenido from "./components/Contenido.vue";
import SobreMi from "./components/SobreMi.vue";
import Proyectos from "./components/Proyectos.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    Contenido,
    SobreMi,
    Proyectos,
  },
};
</script>

<style>
/* @import "./assets/css/w3.css"; */
@import "./assets/css/data.css";
@import "./assets/css/normalize.min.css";
@import "./assets/css/styles.scss";
@import "./assets/css/responsive.css";
</style>
