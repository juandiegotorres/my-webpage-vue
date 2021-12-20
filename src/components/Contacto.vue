<template>
    <section class="contacto__ container mt-3">
        <h3 class="titulo mb-4">Contactáme</h3>
        <form ref="form" @submit.prevent="sendEmail">
            <div class="row justify-content-center">
                <div class="col-10 col-sm-8 col-md-6 col-lg-4 text-center col__mensaje pb-2">
                    <textarea
                        name="mensaje"
                        v-model="mensaje"
                        cols="30"
                        rows="10"
                        class="mensaje__contacto"
                        v-bind:class="{ input__error: error_mensaje }"
                        placeholder="Tu mensaje..."
                    ></textarea>
                    <p class="mensaje__error">{{ error_mensaje }}</p>
                </div>
                <div
                    class="col-10 col-sm-8 col-md-6 col-lg-4 d-flex flex-column justify-content-between col__nombre pb-2"
                >
                    <span class="d-flex flex-column">
                        <input
                            type="text"
                            name="nombre"
                            v-model="nombre"
                            v-bind:class="{ input__error: error_nombre }"
                            placeholder="Nombre..."
                        />
                        <p class="mensaje__error">{{ error_nombre }}</p>
                        <input
                            type="text"
                            v-model="email"
                            name="email"
                            v-bind:class="{ input__error: error_email }"
                            placeholder="E-mail..."
                        />
                        <p class="mensaje__error">{{ error_email }}</p>
                    </span>
                    <button class="btn__primario btn__desktop">Enviar</button>
                </div>
                <div class="col-10 col-sm-8 d-flex flex-column btn__mobile">
                    <button type="submit" class="btn__primario btn__mobile">Enviar</button>
                </div>
            </div>
            <div class="col-12 text-center">
                <p class="mt-3 mb-3">
                    O puedes contactarme a través de mi mail personal
                    <a
                        class="mailto"
                        href="mailto: jdtorres1998@gmail.com"
                    >jdtorres1998@gmail.com</a>
                </p>
            </div>
        </form>
        <div class="notificacion">
            <div class="notificacion__container">
                <img
                    v-bind:src="require('@/assets/images/' + imagen)"
                    class="notificacion__img"
                    alt="img-notificacion"
                />
                <h2 class="notificacion__title">{{ titulo }}</h2>
                <p class="notificacion__paragraph" v-html="texto_notificacion"></p>
                <a class="btn__secundario" v-on:click="cerrarModal">Cerrar</a>
            </div>
        </div>
    </section>
</template>


<script>

import emailjs from 'emailjs-com';

export default {
    data() {
        return {
            nombre: '',
            email: '',
            mensaje: '',
            notificacion: '',
            imagen: 'email_enviado.png',
            titulo: '¡Mensaje enviado!',
            texto_notificacion: 'En cuento lea el correo me pondré en contacto contigo. Muchas gracias :)',
            error_nombre: '',
            error_email: '',
            error_mensaje: '',
            hayError: false,
        }
    },
    mounted() {
        this.notificacion = document.querySelector('.notificacion');
    },
    methods: {
        sendEmail(e) {
            if (this.validarInputs() == false) {
                emailjs.sendForm('service_mnzvl15', 'template_nilcvr1', e.target, 'user_Bq4Dfc09941bP2IilsTdd', {
                    nombre: this.nombre,
                    mensaje: this.mensaje,
                    email: this.email
                }).then((result) => {
                    result;
                    this.borrarErrores();
                    this.notificacion.classList.add('notificacion--show');
                    this.nombre = ''
                    this.email = ''
                    this.mensaje = ''
                }, (error) => {
                    error;
                    this.borrarErrores();
                    this.imagen = '404.png';
                    this.titulo = 'Sucedió un error'
                    this.texto_notificacion = 'El mail no se pudo enviar :( <br> Estoy trabajando para solucionarlo. Mientras tanto puedes contactarme a través de mi correo <a class="mailto" href="mailto: jdtorres1998@gmail.com">jdtorres1998@gmail.com</a>'
                });
            }
        },

        prueba() {
            this.validarInputs()
        },

        validarInputs() {
            this.hayError = false;
            if (!this.nombre || this.nombre.indexOf(' ') >= 0) {
                this.error_nombre = 'El campo nombre no puede estar vacío.';
                this.hayError = true;
            } else {
                this.error_nombre = '';
            }
            if (!this.email || this.email.indexOf(' ') >= 0) {
                this.error_email = 'El campo mail no puede estar vacío.';
                this.hayError = true;
            } else {
                this.error_email = '';
            }
            if (!this.mensaje || this.mensaje.indexOf(' ') >= 0) {
                this.error_mensaje = 'Debes escribir un mensaje.';
                this.hayError = true;
            } else if (this.mensaje.length > 500) {
                this.error_mensaje = 'El límite es de 500 caracteres.';
                this.hayError = true;
            } else {
                this.error_mensaje = '';
            }
            return this.hayError
        },

        borrarErrores() {
            this.error_mensaje = '';
            this.error_nombre = '';
            this.error_email = '';
        },


        cerrarModal() {
            this.notificacion.classList.remove('notificacion--show');
        }
    }
}
</script>