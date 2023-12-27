<script></script>

<template>
    <section class="sobre" id="about">
        <div class="textos">
            <h3>AENEAN CONSECTETUR PORTA</h3>
            <h3>Nullam quis risus eget urna mollis ornare vel eu leo.</h3>
        </div>

        <div class="wrapper">
            <img src="../../public/img/dash-device.png" alt="Imagem do componente sobre">
        </div>
    </section>
</template>

<style scoped>
.sobre {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    background-color: var(--cinza1);
    padding-top: 4.6rem;
}

.textos {
    max-width: 45rem;
    padding: 1rem 1.25rem 2.5rem;
}

.textos h3:first-child {
    font-size: 0.75rem;
    color: var(--cinza5);
    letter-spacing: 2px;
}

.textos h3:last-child {
    font-size: 1.75rem;
    color: var(--branco);
    margin: 1.6rem 0;

    @media (min-width: 768px) {
        font-size: 2.2rem;
    }

    @media (min-width: 1024px) {
        font-size: 2.4rem;
    }
}

.wrapper img {
    max-width: 20rem;
    max-height: 13rem;

    @media (min-width: 768px) {
        max-width: 43rem;
        max-height: 23rem;
    }

    @media (min-width: 1024px) {
        max-width: 57rem;
        max-height: 31rem;
    }

    @media (min-width: 1440px) {
        max-width: 75rem;
        max-height: 40rem;
    }
}

</style>