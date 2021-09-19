<template>
  <div>
    <div class="container">
      <div class="row">
        <div class="col-md-10 mx-auto">
          <h3 class="titulo">Sobre mí</h3>
          <p class="sobre__mi">
            Soy un joven de 23 años de un pequeño pueblo de la provincia de
            Mendoza, hace poco tiempo me recibí como
            <strong>Técnico Analista Programador</strong>
            y estoy en busca de mi primer trabajo como programador donde poder
            demostrar mis conocimientos y poder ayudar a que el usuario tenga la
            mejor experiencia digital. De manera provisoria estoy trabajando
            como desarrollador freelance y comercializando mi propio sistema
            “PractiComercio” como pueden observar más arriba. Mi objetivo es ser
            desarrollador web full stack, algo en lo que estoy trabajando de
            manera autodidacta aprendiendo JavaScript y React junto con otras
            tecnologías. Por cualquier consulta no dudes con contactarme
          </p>
        </div>
      </div>
      <div class="row mt-3">
        <div class="col-md-3">
          <div class="info">
            <div class="icono">
              <font-awesome-icon
                icon="graduation-cap"
                size="5x"
              ></font-awesome-icon>
            </div>
            <div class="descripcion">
              <h4 class="info__titulo">Responsabilidad</h4>
              <p class="info__descripcion">
                Me preocupo por el trabajo de los demás tanto como del mío.
              </p>
              <br />
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="info">
            <div class="icono">
              <font-awesome-icon icon="rocket" size="5x" />
            </div>
            <div class="descripcion">
              <h4 class="info__titulo">Motivación</h4>
              <p class="info__descripcion">
                No me doy por vencido fácilmente y me gustan los retos
                difíciles.
              </p>
              <br />
            </div>
          </div>
        </div>

        <div class="col-md-3">
          <div class="info">
            <div class="icono">
              <font-awesome-icon icon="lightbulb" size="5x" />
            </div>
            <div class="descripcion">
              <h4 class="info__titulo">Soy Autodidacta</h4>
              <p class="info__descripcion">
                Siempre estoy en constante aprendizaje, y me gusta mucho
                investigar por mi cuenta.
              </p>
              <br />
            </div>
          </div>
        </div>
        <div class="col-md-3">
          <div class="info">
            <div class="icono">
              <font-awesome-icon icon="comments" size="5x" />
            </div>
            <div class="descripcion">
              <h4 class="info__titulo">Cooperación</h4>
              <p class="info__descripcion">
                Me gusta el trabajo en equipo, se escuchar y aceptar críticas.
              </p>
              <br />
            </div>
          </div>
        </div>
      </div>
    </div>
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
      <path
        fill="#512DA8"
        fill-opacity="1"
        d="M0,32L34.3,32C68.6,32,137,32,206,58.7C274.3,85,343,139,411,170.7C480,203,549,213,617,192C685.7,171,754,117,823,80C891.4,43,960,21,1029,48C1097.1,75,1166,149,1234,186.7C1302.9,224,1371,224,1406,224L1440,224L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z"
      ></path>
    </svg>
  </div>
</template>

<script>
export default {
  name: "SobreMi",
};
</script>
