<script>
    export default {
        data() {
            return {

            }

        }, 
        methods: {

        }
    }
</script>

<template>
    <section class="banner">
        <div class="box-text">
            <h2 class="titulo">Momentum</h2>
            <h3 class="texto">Lounch your product - and savor the momentum.</h3>
            <a href="#download" class="btn-get">Get the App</a>
        </div>

        <div>
            <!-- arrow -->
        </div>
    </section>

</template>

<style scoped>
.banner {
    display: flex;
    flex-direction: column;
    padding: 15rem 0 0 2rem;
    height: 100vh;
    background-image: linear-gradient(135deg, var(--rosa2), var(--roxo1));
    
    @media (min-width: 992px) {
        padding: 14rem 0 0 8rem;
    }
}

.box-text {
    color: var(--branco);
    font-weight: bold;
}

.titulo {
    font-size: 2.6rem;
    margin-bottom: 1.5rem;

    @media (min-width: 992px) {
        font-size: 3.8rem; 
        font-weight: 700;
    }
}   

.texto {
    font-size: 1.6rem;
    margin: .6rem 0 2.5rem 0;
    line-height: 1.9rem;
    max-width: 55vw;

    @media (min-width: 992px) {
        font-weight: 400;
        font-size: 2.1rem;
        margin-bottom: 3rem;
    }
}

.btn-get {
    font-size: 1rem;
    color: var(--branco);
    background-color: var(--rosa1);
    padding: 1.25rem 2.5rem;
    font-weight: bold;
    text-decoration: none;
    transition: bic-bezier(.789, .159, .25, 1);
    transition: background-color 500ms cubic-bezier(.789, .159, .25, 1), color 200ms cubic-bezier(.789, .159, .25, 1);
    
    @media (min-width: 992px) {
        padding: 1.5rem 2.5rem;
        border-radius: 3px;
    }

    &:hover {
        background-color: var(--branco);
        color: var(--cinza4);
    }
    
}


</style>