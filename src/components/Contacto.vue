<template>
    <section class="contacto__ container">
        <h3 class="titulo mb-4">Contactáme</h3>
        <div class="row justify-content-center">
            <div class="col-10 col-sm-8 col-md-6 col-lg-4 text-center col__mensaje pb-2">
                <textarea
                    name="mensaje"
                    id
                    cols="30"
                    rows="10"
                    class="mensaje__contacto"
                    placeholder="Tu mensaje..."
                ></textarea>
            </div>
            <div
                class="col-10 col-sm-8 col-md-6 col-lg-4 d-flex flex-column justify-content-between col__nombre pb-2"
            >
                <span class="d-flex flex-column">
                    <input type="text" name="nombre" class="mb-2" placeholder="Nombre..." />
                    <input type="text" name="email" class placeholder="E-mail..." />
                </span>
                <button class="btn__primario btn__desktop">Enviar</button>
            </div>
            <div class="col-10 col-sm-8 d-flex flex-column btn__mobile">
                <button class="btn__primario btn__mobile">Enviar</button>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>