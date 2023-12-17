<script></script>

<template>
    <section class="recursos">
        <div class="recursosBox">
            <div class="recursosBoxTexto">
                <h3 class="titulo">AENEAN CONSECTETUR</h3>
                <h3 class="subtitulo">Cay sociis nato que penatibus et</h3>
                <p class="texto">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.</p>
            </div>
            <img src="../../public/img/app-06.png" alt="">
        </div>

        <div class="recursosBox">
            <img src="../../public/img/app-05.png" alt="">
            <div class="recursosBoxTexto">
                <h3 class="titulo">CONSECTULTRICIES</h3>
                <h3 class="subtitulo">Amet Ipsum</h3>
                <p class="texto">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.</p>
            </div>
        </div>

        <div class="recursosBox">
            <div class="recursosBoxTexto">
                <h3 class="titulo">AENEAN CONSECTETUR PORTA</h3>
                <h3 class="subtitulo">Magna Porta Sit Bibendum</h3>
                <p class="texto">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.</p>
            </div>
            <img src="../../public/img/app-04.png" alt="" >
        </div>
    </section>
</template>

<style scoped>
.recursos {
    margin: 4rem 0;
    padding: 0 1rem;
    display: flex;
    flex-direction: column;
    gap: 5rem;
}

.recursosBox {
    display: flex;
    flex-direction: column;

    &:nth-child(2) {
        flex-direction: column-reverse;

        @media (min-width: 768px) {
            flex-direction: row;
            align-items: center;
            justify-content: center;
        img {
            max-width: 19rem;
        }
    }
    }

    @media (min-width: 768px) {
        flex-direction: row;
        align-items: center;
        justify-content: center;

        img {
            max-width: 19rem;
        }
    }
}   

.recursosBoxTexto {
    padding: 0 1rem;
    max-width: 25rem;
}

.titulo {
    padding-bottom: 5px;
    font-size: 0.7rem;
    color: #a8a8a8;
    letter-spacing: 2px;
}

.subtitulo {
    margin: 1.2rem 0;
    font-size: 1.7rem;
    color: #000;

    @media (min-width: 768px) {
        font-size: 2.3rem;
    }
}

.texto {
    margin-bottom: 0.6rem;
    font-size: 1rem;
    color: #6b6b6b;
    line-height: 1.8rem;
}


</style>