<template>
  <div>
    <div class="content">
      <span class="bienvenida__">
        <!-- <ul>
          <li class="titulo__bienvenida">Bienvenido</li>
          <li class="titulo__bienvenida">Bienvenida</li>
          <li class="titulo__bienvenida">Bienvenidx</li>
        </ul>-->
        <h1 class="titulo__bienvenida">
          Bienvenid
          <span class="texto__tipeado">{{ valor }}</span>
          <span class="cursor__" :class="{ 'tipeando': estado }">&nbsp;</span>
          <br />a mi página web
        </h1>
        <h5 class="subtitulo__bienvenida">Mi nombre es Juan y soy Analista-Programador de sistemas</h5>
        <span class="redes__">
          <a href="https://www.instagram.com/juandtorres0/" target="_blank">
            <img
              src="https://icongr.am/entypo/instagram.svg?size=128&color=ffffff"
              alt
              class="icono__redes"
            />
          </a>
          <a href="https://www.linkedin.com/in/jtdeveloper/" target="_blank">
            <img
              src="https://icongr.am/entypo/linkedin.svg?size=128&color=ffffff"
              alt
              class="icono__redes"
            />
          </a>
          <a href="https://github.com/juandiegotorres/" target="_blank">
            <img
              src="https://icongr.am/fontawesome/github.svg?size=128&color=ffffff"
              alt
              class="icono__redes"
            />
          </a>
        </span>
      </span>
      <span class="contenedor__imagen">
        <img :src="require('@/assets/images/developer1.svg')" alt class="img__inicio" />
      </span>
    </div>

    <div class="spacer curva__1"></div>
  </div>
</template>
<script>

export default {
  name: "Contenido",

  data() {
    return {
      valor: "",
      estado: false,
      arrayLetras: ["o", "a", "x"],
      velocidadTipeado: 400,
      velocidadBorrado: 100,
      delayNuevaLetra: 2000,
      arrayLetrasIndex: 0,
      letraIndex: 0,
    };
  },


  mounted() {
  },

  methods: {
    tipearTexto() {
      if (this.letraIndex < this.arrayLetras[this.arrayLetrasIndex].length) {
        if (!this.estado)
          this.estado = true;
        this.valor += this.arrayLetras[this.arrayLetrasIndex].charAt(this.letraIndex);
        this.letraIndex += 1;
        setTimeout(this.tipearTexto, this.velocidadTipeado);
      }
      else {
        this.estado = false;
        setTimeout(this.borrarTexto, this.delayNuevaLetra);
      }
    },

    borrarTexto() {
      if (this.letraIndex > 0) {
        if (!this.estado)
          this.estado = true;
        this.valor = this.arrayLetras[this.arrayLetrasIndex].substring(0, this.letraIndex - 1);
        this.letraIndex -= 1;
        setTimeout(this.borrarTexto, this.velocidadBorrado);
      }
      else {
        this.estado = false;
        this.arrayLetrasIndex += 1;
        if (this.arrayLetrasIndex >= this.arrayLetras.length)
          this.arrayLetrasIndex = 0;
        setTimeout(this.tipearTexto, this.velocidadTipeado + 1000);
      }
    }
  },

  created() {
    setTimeout(this.tipearTexto, this.delayNuevaLetra + 200);
  }
};
</script>
