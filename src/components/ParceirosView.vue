<script></script>

<template>
    <section class="parceiros">

        <!-- Carousel com feedbacks -->
        <div></div>

        <img src="../../public/img/parceiros.png" alt="Parceiros da Richard" class="imgParceiros">
        <img src="../../public/img/apps-banner.jpeg" alt="Banner do app Richard" class="imgApp">
    </section>
</template>

<style scoped>

.parceiros {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.imgParceiros {
    padding: 3.4rem 1rem;
    max-width: 18rem;

    @media (min-width: 425px) {
        max-width: 23.9rem;
    }

    @media (min-width: 768px) {
        max-width: 43.2rem;
    }

    @media (min-width: 1024px) {
        max-width: 45rem;
    }

    @media (min-width: 1440px) {
        max-width: 63rem;
    }
}

.imgApp {
    width: 100%;
    max-height: 32.4rem;
}

</style>