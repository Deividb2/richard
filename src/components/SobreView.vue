<script></script>

<template>
    <section class="sobre">
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
    background-color: #1b1b1b;
    padding-top: 73px;
}

.textos {
    max-width: 45rem;
    padding: 16px 20px 40px;
}

.textos h3:first-child {
    font-size: 12px;
    color: #a8a8a8;
    letter-spacing: 2px;
}

.textos h3:last-child {
    font-size: 28px;
    color: #fff;
    margin: 25px 0;

    @media (min-width: 768px) {
        font-size: 34px;
    }

    @media (min-width: 1024px) {
        font-size: 38px;
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