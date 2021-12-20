<template>
    <section>
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" class="curva__footer">
            <path
                fill="#512da8"
                fill-opacity="1"
                d="M0,224L80,218.7C160,213,320,203,480,213.3C640,224,800,256,960,256C1120,256,1280,224,1360,208L1440,192L1440,320L1360,320C1280,320,1120,320,960,320C800,320,640,320,480,320C320,320,160,320,80,320L0,320Z"
            />
        </svg>
        <footer>
            <div class="d-flex flex-column mb-3">
                <p class="texto__footer">
                    <strong>Pagina web hecha a base de muchos mates 🧉</strong>
                </p>
                <p>&copy; Juan Diego Torres | 2022</p>
            </div>
            <div class="d-flex justify-content-between redes__footer pb-2">
                <a
                    href="https://www.instagram.com/juandtorres0/"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    <img
                        :src="require('@/assets/images/instagram(2).svg')"
                        class="ml-3 mr-3"
                        alt="Instagram"
                    />
                </a>

                <a
                    href="https://github.com/juandiegotorres/"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    <img :src="require('@/assets/images/github(1).svg')" class="mr-3" alt="Github" />
                </a>
                <a
                    href="https://www.linkedin.com/in/jtdeveloper/"
                    target="_blank"
                    rel="noopener noreferrer"
                >
                    <img :src="require('@/assets/images/linkedin.svg')" class="mr-3" alt="LinkedIn" />
                </a>
            </div>
        </footer>
    </section>
</template>

<script>
export default {

}
</script>
