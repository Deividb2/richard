<script></script>

<template>
    <section class="comida" id="how-to-use">
        <div class="comidaBox">
            <div class="boxTexto">       
                <h3 class="titulo">AENEAN CONSECTETUR PORTA</h3>
                <h3 class="subtitulo">Sem Risus Elit Vestibulum</h3>
                <p class="texto">Nulla vitae elit libero, a pharetra augue. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. <a href="#">Cras mattis consectetur</a> purus sit amet fermentum. Donec id elit non mi porta gravida at eget metus. Etiam porta sem malesuada magna mollis euismod.</p>
            </div>
            <div class="imgs imgBurger"></div>
        </div>

        <div  class="comidaBox">
            <div class="boxTexto">       
                <h3 class="titulo">AENEAN CONSECTETUR PORTA</h3>
                <h3 class="subtitulo">Parturient Tortor</h3>
                <p class="texto">Nulla vitae elit libero, a pharetra augue. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. <a href="#">Cras mattis consectetur</a> purus sit amet fermentum. Donec id elit non mi porta gravida at eget metus. Etiam porta sem malesuada magna mollis euismod.</p>
            </div>
            <div class="imgs imgSalada"></div>
        </div>
    </section>
</template>

<style scoped>

.comida {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 4rem 0;
    padding: 0 1rem;
    gap: 3rem;
    
    @media (min-width: 768px) {
        gap: 6rem;
    }

    @media (min-width: 1440px) {
        gap: 8rem;
    }
}   

.comidaBox {
    padding: 0.75rem;

    @media (min-width: 768px) {
        display: flex;
        align-items: center;
        
        &:nth-child(2) {
            flex-direction: row-reverse;
        }
    }
}

.boxTexto {
    max-width: 20rem;
    
    @media (min-width: 768px) {
        padding: 0 1.8rem;
        max-width: 30rem;
    }

    @media (min-width: 1440px) {
        padding: 0 3.5rem;
    }
}

.titulo {
    padding-bottom: 5px;
    font-size: 0.7rem;
    color: var(--cinza5);
    letter-spacing: 2px;
}

.subtitulo {
    margin: 1.2rem 0;
    font-size: 1.7rem;
    color: var(--preto);

    @media (min-width: 768px) {
        font-size: 2.3rem;
    }
}

.texto {
    margin-bottom: 1.2rem;
    font-size: 1rem;
    color: var(--cinza4);
    line-height: 1.9rem;

    a {
        color: var(--preto);
    }
}

.imgs {
    min-width: 18rem;
    max-width: 23.8rem;
    min-height: 15rem;
    max-height: 20rem;

    @media (min-width: 1024px) {
        min-width: 32.5rem;
        min-height: 25.9rem;
    }
}

.imgBurger {
    background: url(../../public/img/img-03.jpeg) no-repeat center / cover;
}   

.imgSalada {
    background: url(../../public/img/img-02.jpeg) no-repeat center / cover;
}

</style>