<script>
import BurgerIcon from '../../public/img/icon-burger.svg'
import DataIcon from '../../public/img/icon-data.svg'
import SilverIcon from '../../public/img/icon-silverware.svg'
    export default {
        data() {
            return {
                icone1: BurgerIcon,
                icone2: DataIcon,
                icone3: SilverIcon,

                dadosGerais: [
                    {
                        icon: BurgerIcon,
                        alt: 'Ícone de hambúger',
                        titulo: 'Activity Notifications',
                        texto: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.'
                    },
                    {
                        icon: SilverIcon,
                        alt: 'Ícone de talheres',
                        titulo: 'Custom Timing',
                        texto: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.'
                    },
                    {
                        icon: DataIcon,
                        alt: 'Ícone de gráfico',
                        titulo: 'Mobile Optimized',
                        texto: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.'
                    }
                ],
                dadosNumeros: [
                    {
                        numero: '+12k',
                        titulo: 'Nibh Elit Tristique'
                    },
                    {
                        numero: '84',
                        titulo: 'Aenean Condimentum'
                    },
                    {
                        numero: '3,07',
                        titulo: 'Quam Inceptos'
                    },
                    {
                        numero: '24h',
                        titulo: 'Ullamcorper'
                    }
                ],
            }
        }
    }
</script>

<template>
    <section class="metricas">
        <div class="metricasGerais">
            <div v-for="(elemento, index) in dadosGerais" v-bind:key="index" class="geraisBox">
                <img :src="elemento.icon" :alt="elemento.alt" class="geraisImg">
                <h4 class="geraisTitulo">{{ elemento.titulo }}</h4>
                <h5 class="geraisTexto">{{ elemento.texto }}</h5>
            </div>
        </div>

        <div class="metricasNumericas">
            <div v-for="(elemento, index) in dadosNumeros" :key="index" class="numericasBox">
                <h5 class="numericasNumero">{{ elemento.numero }}</h5>
                <h4 class="numericasTitulo">{{ elemento.titulo }}</h4>
            </div>
        </div>
    </section>
</template>

<style scoped>
.metricas {
    display: flex;
    flex-direction: column;
    padding: 2.6rem 1rem;
    @media (min-width: 768px) {
        gap: 3.5rem;
    }
}

/* DADOS GERAIS */
.metricasGerais {    
    margin: 3rem 0;
    @media (min-width: 768px) {
        display: flex;
        margin: 3.7rem;
    }
}

.geraisBox {
    padding-bottom: 1.8rem;

    @media (min-width: 768px) {
        padding: 0 1.8rem;
        text-align: center;
    }
}

.geraisImg {
    margin-bottom: 1.25rem;
    width: 80px;
    height: 35px;
}

.geraisTitulo {
    margin: 0.6rem 0; 
    color: #000;
    font-size: 1.1rem;
}

.geraisTexto {
    margin-bottom: 0.6rem;
    color: #6b6b6b;
    font-size: 1rem;
    line-height: 1.8rem;
}

/* DADOS NUMÉRICOS */

.metricasNumericas {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 1rem;
    margin: 5rem 0;

    @media (min-width: 768px) {
        grid-template-columns: repeat(4, 1fr);
        margin: 0;
    }
}

.numericasBox {
    padding: 0 0.9rem 1.8rem 0.9rem;
    text-align: center;

    @media (min-width: 768px) {
        padding: 0 1.8rem;
    }
}

.numericasNumero {
    font-size: 2.5rem;
    font-weight: 400;
    color: #333333; 

    @media (min-width: 768px) {
        font-size: 3.7rem;
        font-weight: 500;
    }
}

.numericasTitulo {
    font-size: 1.1rem;
    font-weight: 700;
    text-align: center;
    color: #000; 
    line-height: 1.5rem;
    margin: 0.6rem 0;
}

</style>