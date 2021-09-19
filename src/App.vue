<template>
  <div id="app">
    <HeaderComponent></HeaderComponent>
    <Contenido></Contenido>
    <SobreMi></SobreMi>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import Contenido from "./components/Contenido.vue";
import SobreMi from "./components/SobreMi.vue";

export default {
  name: "App",
  components: {
    HeaderComponent,
    Contenido,
    SobreMi,
  },
};
</script>

<style>
@import "./assets/css/styles.css";
</style>
