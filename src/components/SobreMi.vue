<template>
  <section class="mt-3">
    <div class="container">
      <h3 class="titulo">Sobre mí</h3>
      <div class="row">
        <div class="col-md-10 sss">
          <div class="sobre__mi">
            <p>¡Hola! Mi nombre es Juan Diego Torres y tengo 23 años. Soy un apasionado por la computación y todo lo que la rodea.</p>
            <br />
            <p>
              En plena pandemia me recibí como
              <b>técnico analista programador</b> y algunos meses después conseguí mi primer trabajo como programador full-stack. Actualmente, me encuentro trabajando con tecnologías como
              <b>Laravel, MySQL, Bootstrap, jQuery y más.</b>
            </p>
            <br />
            <p>
              Mi objetivo a corto plazo es continuar
              <b>aprendiendo</b> sobre la construcción de
              <b>API RESTful</b> y su utilización, algo que desde hace tiempo me atrae mucho y tengo ganas de realizar proyectos con base en esto.
            </p>
            <br />
            <p>
              <b>Siempre tengo como finalidad poder desempeñar mis labores de la mejor forma posible, con ganas de crecer, pero sobre todo de seguir aprendiendo día a día de cada persona y cada experiencia.</b>
            </p>
          </div>
          <!-- <b-button v-b-modal.modal-scrollable class="btn-curriculum">Launch demo modal</b-button> -->
        </div>
        <div class="col-md-6 d-flex mx-auto justify-content-center mb-3">
          <button class="btn__secundario" id="myBtn" @click="showModal = true">Ver curriculum</button>
        </div>
      </div>
      <!-- ================SKILLS================== -->

      <!-- ==================MODAL CURRICULUM=================== -->
      <div class="modal" id="myModal">
        <!-- Modal content -->
        <div class="modal-content">
          <span class="close">&times;</span>
          <div class="row justify-content-center">
            <div class="contenedor__img__curriculum">
              <img
                :src="require('@/assets/images/foto_perfil.jpg')"
                alt="Foto de perfil"
                class="img__perfil"
              />
            </div>
            <div class="presentacion__curriculum">
              <h2 class>Juan Diego Torres</h2>
              <h4>Analista-programador JR</h4>
            </div>
          </div>
          <div class="row justify-content-center">
            <div class="col-lg-6 col-md-8">
              <!--=============== SOBRE MI =============== -->
              <div class="sobremi__curriculum">
                <h3 class="text-center">Sobre mi</h3>
                <p class="mt-2">
                  <strong>Edad:</strong>
                </p>
                <p>23 años</p>
                <p class="mt-2">
                  <strong>Email:</strong>
                </p>
                <p>
                  <a
                    href="mailto:jdtorres1998@gmail.com"
                    target="_blank"
                    rel="noopener noreferrer"
                  >jdtorres1998@gmail.com</a>
                </p>
                <p class="mt-2">
                  <strong>Lugar de residencia:</strong>
                </p>
                <p>San Rafael (Mendoza) - Argentina</p>
              </div>
              <!-- ============= FORMACION ============= -->
              <div class="formacion__curriculum">
                <h3 class="text-center">Formación</h3>
                <p class="mb-1 mt-2">
                  <strong>Educacion terciaria (IES 9-012)</strong>
                </p>
                <li>Técnico superior en análisis y programación de sistemas</li>
                <li>Marzo 2017 - Diciembre 2020</li>
                <h4 class="mt-2 mb-2">Cursos:</h4>
                <p class="mb-1">
                  <strong>Ingles aplicado a las TICS</strong>
                </p>
                <li>Instituto Santa Trinidad</li>
                <li>Octubre 2020 - Diciembre 2020</li>
                <p class="mt-2">
                  <strong>JAVA</strong>
                </p>
                <li>Instituto Santa Trinidad</li>
                <li>Agosto 2019 - Diciembre 2019</li>
              </div>
            </div>
            <div class="col-lg-6 col-md-8">
              <!-- ========= EXPERIENCIA LABORAL ============= -->
              <div class="experiencia__curriculum">
                <h3 class="text-center">Experiencia laboral</h3>
                <p class="mt-2">
                  <strong>Desarrollador Web</strong>
                </p>
                <p>
                  <a
                    href="https://www.instagram.com/dilook.media/"
                    target="_blank"
                    rel="noopener"
                  >Dilook Media</a>
                </p>
                <p class="mb-1">Agosto 2021 - Actualidad</p>
                <li>Desarrollo de sistemas de gestión web a medida para empresas</li>
                <li>Desarrollo de páginas web con Laravel, CSS y Boostrap</li>

                <p class="mt-2">
                  <strong>Freelance</strong>
                </p>
                <p>'PractiComercio'</p>
                <p class="mb-1">Desde Marzo 2021 - Julio 2021</p>
                <li>Diseño y comercialización de software de sistema de ventas y control de stock para pequeños y medianos comercios</li>

                <p class="mt-2">
                  <strong>Reparador de PC's</strong>
                </p>
                <p>360 IT - Soluciones informáticas</p>
                <p>Desde Mayo 2019 - Enero 2021</p>
              </div>
              <!-- ============ IDIOMAS ========= -->
              <div class="idiomas__curriculum">
                <h3 class="text-center mb-1">Idiomas</h3>
                <p>
                  <strong>Español</strong>
                </p>
                <li>Nativo</li>
                <p class="mt-1">
                  <strong>Inglés</strong>
                </p>
                <li>Intermedio - Avanzado</li>
              </div>
            </div>
            <!-- <div class="col-md-8 col-lg-12">
              <div class="skills__curriculum">
                <h4>Habilidades:</h4>
                <p class="mt-2">
                  <strong>Frontend y otros</strong>
                </p>
                <li>HTML 5</li>
                <li>CCS 3</li>
                <li>JavaScript</li>
                <li>Boostrap</li>
                <li>Vue.js</li>
                <li>jQuery (Libreria)</li>

                <p class="mt-2">
                  <strong>Backend y otros</strong>
                </p>
                <li>PHP</li>
                <li>Laravel</li>
                <li>MySQL</li>

                <p class="mt-2">
                  <strong>Otros</strong>
                </p>
                <li>VB.NET</li>
              </div>
            </div>-->
          </div>
          <!-- =========== BTN DESCARGAR CURRICULUM ============ -->
          <div class="row justify-content-center mt-3 mb-2">
            <a
              href="Juan Diego Torres - CV.pdf"
              class="btn__primario"
              download
            >Descargar curriculum en PDF</a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SobreMi",
  data() {
    return {
      showModal: false
    }
  },
  mounted() {
    var modal = document.getElementById("myModal");

    var modalBody = document.querySelector('.modal-content');
    // Get the button that opens the modal
    var btn = document.getElementById("myBtn");

    // Get the <span> element that closes the modal
    var span = document.getElementsByClassName("close")[0];

    // When the user clicks on the button, open the modal
    btn.onclick = function () {
      modalBody.classList.add('modal__activo');
      modal.classList.add('modal__activo');
    }

    // When the user clicks on <span> (x), close the modal
    span.onclick = function () {
      modalBody.classList.remove('modal__activo');
      setTimeout(function () {
        modal.classList.remove('modal__activo');
      }, 500);
    }

    // When the user clicks anywhere outside of the modal, close it
    window.onclick = function (event) {
      if (event.target == modal) {
        span.click();
      }
    }
  }
};
</script>
