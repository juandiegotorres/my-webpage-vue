<template>
    <div class="proyectos__" id="probando">
        <div class="container pb-5">
            <h3 class="titulo">Mis proyectos</h3>

            <div class="row justify-content-center">
                <div class="col-md-3 mb-4 mb-md-0">
                    <div class="img__container">
                        <img
                            :src="require('@/assets/images/recetardas2.webp')"
                            class="img__proyecto"
                            alt
                        />
                    </div>
                    <div class="card__body__proyecto text-center">
                        <h1>"Red social" de recetas</h1>
                        <p class="sub__tecnologias">BOOTSTRAP - VUE.js - LARAVEL - MySQL</p>
                        <div class="col-md-12 d-flex justify-content-center">
                            <a
                                hrer="https://github.com/juandiegotorres/rsRecetas"
                                target="_blank"
                                class="btn btn-secondary btn-rounded mx-1"
                            >
                                Repositorio
                                <img
                                    src="https://icongr.am/entypo/github.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                            <a href class="btn btn-danger btn-yt btn-rounded mx-1">
                                Youtube
                                <img
                                    src="https://icongr.am/entypo/youtube.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 mb-4 mb-md-0">
                    <div class="img__container">
                        <img
                            :src="require('@/assets/images/market.webp')"
                            class="img__proyecto"
                            alt
                        />
                    </div>
                    <div class="card__body__proyecto text-center">
                        <h1>Sistema de pedidos online</h1>
                        <p class="sub__tecnologias">BOOTSTRAP - LARAVEL - MySQL</p>
                        <p>Página web de pedidos online, con inicio de sesión y registro de clientes. ABM de productos con cuenta administrador y envio de mails</p>
                        <div class="col-md-12 d-flex justify-content-center">
                            <a
                                href="https://github.com/juandiegotorres/market"
                                target="_blank"
                                class="btn btn-secondary btn-rounded mx-1"
                            >
                                Repositorio
                                <img
                                    src="https://icongr.am/entypo/github.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                            <a
                                href="https://www.youtube.com/watch?v=BElDnhk5mTo"
                                target="_blank"
                                class="btn btn-danger btn-yt btn-rounded mx-1"
                            >
                                Youtube
                                <img
                                    src="https://icongr.am/entypo/youtube.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 mb-4 mb-md-0">
                    <div class="img__container">
                        <img :src="require('@/assets/images/360it.webp')" class="img__proyecto" alt />
                    </div>
                    <div class="card__body__proyecto text-center">
                        <h1>Software de gestión</h1>
                        <br />
                        <p class="sub__tecnologias">VB.NET - MySQL</p>
                        <br />
                        <p>Software de gestión de ventas, control de stock, proveedores, clientes y un módulo para registrar reparaciones de PC</p>
                        <div class="col-md-12 d-flex justify-content-center">
                            <a
                                href="https://github.com/juandiegotorres/360it"
                                target="_blank"
                                class="btn btn-secondary btn-rounded mx-1"
                            >
                                Repositorio
                                <img
                                    src="https://icongr.am/entypo/github.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                            <a
                                href="https://www.youtube.com/watch?v=sCKmvYnbP0c"
                                target="_blank"
                                class="btn btn-danger btn-yt btn-rounded mx-1"
                            >
                                Youtube
                                <img
                                    src="https://icongr.am/entypo/youtube.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row justify-content-center mt-md-5">
                <div class="col-md-3 mb-4 mb-md-0">
                    <div class="img__container">
                        <img
                            :src="require('@/assets/images/crudJS.webp')"
                            class="img__proyecto"
                            alt
                        />
                    </div>
                    <div class="card__body__proyecto text-center">
                        <h1>Crud JavaScript</h1>
                        <p class="sub__tecnologias">JavaScript Vanilla</p>
                        <p>Mis primeros contactos con JavaScript. CRUD sencillo usando local storage</p>
                        <div class="col-md-12 d-flex justify-content-center">
                            <a
                                href="https://github.com/juandiegotorres/360it"
                                target="_blank"
                                class="btn btn-secondary btn-rounded mx-1"
                            >
                                Repositorio
                                <img
                                    src="https://icongr.am/entypo/github.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                            <a
                                href="https://juandiegotorres.github.io/CRUD_JS/"
                                target="_blank"
                                class="btn btn-success btn-rounded mx-1"
                            >
                                Visitar
                                <img
                                    src="https://icongr.am/fontawesome/external-link.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 mb-4 mb-md-0">
                    <div class="img__container">
                        <img
                            :src="require('@/assets/images/entregaTurnos.webp')"
                            class="img__proyecto"
                            alt
                        />
                    </div>
                    <div class="card__body__proyecto text-center">
                        <h1>Software de gestión de turnos</h1>
                        <p class="sub__tecnologias">VB.NET - MySQL</p>
                        <p>Software de gestión de turnos de un salón de fiestas, control de clientes, extras, turnos y módulo de reportes con gráficos</p>
                        <div class="col-md-12 d-flex justify-content-center">
                            <a
                                href="https://github.com/juandiegotorres/360it"
                                target="_blank"
                                class="btn btn-secondary btn-rounded mx-1"
                            >
                                Repositorio
                                <img
                                    src="https://icongr.am/entypo/github.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                            <a
                                href="https://www.youtube.com/watch?v=-Y-Z1FBpCOM"
                                target="_blank"
                                class="btn btn-danger btn-yt btn-rounded mx-1"
                            >
                                Youtube
                                <img
                                    src="https://icongr.am/entypo/youtube.svg?size=16&color=ffffff"
                                    alt
                                    class="icono__16px"
                                />
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>