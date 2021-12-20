<template>
    <section>
        <div class="proyectos__">
            <div class="container pb-5">
                <h3 class="titulo">Mis proyectos</h3>

                <div class="row justify-content-center pb-4">
                    <div class="col-11 col-sm-8 col-md-6 col-lg-4 col-xl-4 mb-4 mb-md-0 card__">
                        <!-- =============== IMG CARD 1 ============= -->
                        <div class="sombra__card">
                            <div class="img__container">
                                <img
                                    :src="require('@/assets/images/recetardas2 (2).png')"
                                    class="img__proyecto"
                                    alt="Recetardas"
                                />
                            </div>
                            <!-- ============= CARD 1 ============== -->
                            <div class="card__body__proyecto text-center">
                                <div>
                                    <p class="tit__proyecto">"Red social" de recetas</p>
                                    <p class="sub__tecnologias">BOOTSTRAP - VUE.js - LARAVEL - MySQL</p>
                                    <p
                                        class="descripcion__proyecto"
                                    >Página web de recetas, con autenticación y sistema de likes en las recetas. CRUD de recetas con subida de imágenes y visualización de perfiles</p>
                                </div>
                                <div class="col-12 d-flex justify-content-center">
                                    <a
                                        href="https://www.github.com/juandiegotorres/rsRecetas"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__git btn__sm"
                                    >Repositorio</a>
                                    <a
                                        href="https://www.youtube.com/watch?v=3v-aD2rvidI"
                                        class="btn__yt btn__sm"
                                    >Youtube</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-11 col-sm-8 col-md-6 col-lg-4 col-xl-4 mb-4 mb-md-0 card__">
                        <!-- =============== IMG CARD 2 ============= -->
                        <div class="sombra__card">
                            <div class="img__container">
                                <img
                                    :src="require('@/assets/images/market (2).png')"
                                    class="img__proyecto"
                                    alt="Pedidos online"
                                />
                            </div>
                            <!-- =============== CARD 2 ============= -->
                            <div class="card__body__proyecto text-center">
                                <div>
                                    <p class="tit__proyecto">Sistema de pedidos online</p>
                                    <p class="sub__tecnologias">BOOTSTRAP - LARAVEL - MySQL</p>
                                    <p
                                        class="descripcion__proyecto"
                                    >Página web de pedidos online, con inicio de sesión y registro de clientes. ABM de productos con cuenta administrador y envio de mails</p>
                                </div>
                                <div class="col-md-12 d-flex justify-content-center">
                                    <a
                                        href="https://www.github.com/juandiegotorres/market"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__git btn__sm"
                                    >Repositorio</a>
                                    <a
                                        href="https://www.youtube.com/watch?v=BElDnhk5mTo"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__yt btn__sm"
                                    >Youtube</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-11 col-sm-8 col-md-6 col-lg-4 col-xl-4 mb-4 mb-md-0 card__">
                        <!-- =============== IMG CARD 3 ============= -->
                        <div class="sombra__card">
                            <div class="img__container">
                                <img
                                    :src="require('@/assets/images/360it (2).png')"
                                    class="img__proyecto"
                                    alt="Software gestion"
                                />
                            </div>
                            <!-- =============== CARD 3 ============= -->
                            <div class="card__body__proyecto text-center">
                                <div>
                                    <p class="tit__proyecto">Software de gestión</p>
                                    <p class="sub__tecnologias">VB.NET - MySQL</p>
                                    <p
                                        class="descripcion__proyecto"
                                    >Software de gestión de ventas, control de stock, proveedores, clientes y un módulo para registrar reparaciones de PC</p>
                                </div>
                                <div class="col-md-12 d-flex justify-content-center">
                                    <a
                                        href="https://www.github.com/juandiegotorres/360it"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__git btn__sm"
                                    >Repositorio</a>
                                    <a
                                        href="https://www.youtube.com/watch?v=sCKmvYnbP0c"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__yt btn__sm"
                                    >Youtube</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- </div> -->
                    <!-- <div class="row justify-content-center mt-md-5"> -->
                    <div class="col-11 col-sm-8 col-md-6 col-lg-4 col-xl-4 mb-4 card__">
                        <!-- =============== IMG CARD 4 ============= -->
                        <div class="sombra__card">
                            <div class="img__container">
                                <img
                                    :src="require('@/assets/images/crudJS (2).png')"
                                    class="img__proyecto"
                                    alt="CRUD JavaScript"
                                />
                            </div>
                            <!-- =============== CARD 4 ============= -->
                            <div class="card__body__proyecto text-center">
                                <div>
                                    <p class="tit__proyecto">Crud JavaScript</p>
                                    <p class="sub__tecnologias">JavaScript Vanilla</p>
                                    <p
                                        class="descripcion__proyecto"
                                    >Mis primeros contactos con JavaScript. CRUD sencillo usando local storage</p>
                                </div>
                                <div class="col-md-12 d-flex justify-content-center">
                                    <a
                                        href="https://www.github.com/juandiegotorres/360it"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__git btn__sm"
                                    >Repositorio</a>
                                    <a
                                        href="https://juandiegotorres.github.io/CRUD_JS/"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__verde btn__sm"
                                    >Visitar</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-11 col-sm-8 col-md-6 col-lg-4 col-xl-4 mb-3 card__">
                        <!-- =============== IMG CARD 5 ============= -->
                        <div class="sombra__card">
                            <div>
                                <div class="img__container">
                                    <img
                                        :src="require('@/assets/images/entregaTurnos (2).png')"
                                        class="img__proyecto"
                                        alt="Gestion de turnos"
                                    />
                                </div>
                            </div>
                            <!-- =============== CARD 5 ============= -->
                            <div class="card__body__proyecto text-center">
                                <div>
                                    <p class="tit__proyecto">Software de gestión de turnos</p>
                                    <p class="sub__tecnologias">VB.NET - MySQL</p>
                                    <p
                                        class="descripcion__proyecto"
                                    >Software de gestión de turnos de un salón de fiestas, control de clientes, extras, turnos y módulo de reportes con gráficos</p>
                                </div>
                                <div class="col-md-12 d-flex justify-content-center">
                                    <a
                                        href="https://www.github.com/juandiegotorres/360it"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__git btn__sm"
                                    >Repositorio</a>
                                    <a
                                        href="https://www.youtube.com/watch?v=-Y-Z1FBpCOM"
                                        target="_blank"
                                        rel="noopener noreferrer"
                                        class="btn__yt btn__sm"
                                    >Youtube</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path
                fill="#512da8"
                fill-opacity="1"
                d="M0,224L48,240C96,256,192,288,288,277.3C384,267,480,213,576,181.3C672,149,768,139,864,149.3C960,160,1056,192,1152,213.3C1248,235,1344,245,1392,250.7L1440,256L1440,0L1392,0C1344,0,1248,0,1152,0C1056,0,960,0,864,0C768,0,672,0,576,0C480,0,384,0,288,0C192,0,96,0,48,0L0,0Z"
            />
        </svg>
    </section>
</template>

<script>
export default {

}
</script>