<script></script>

<template>
    <section class="newsletter" id="download">
        <div class="baixar">
            <h3 class="baixarTitulo">Ready to get started?</h3>
            <div class="baixarBtnBox">
                <button>Download Now</button>
                <a href="#contato">Get it Touch</a>
            </div>
        </div>

        <div class="contato" id="contato">
            <h3 class="contatoTitulo">Get updates from Richard</h3>
            <h4 class="contatoSubtitulo">New course alerts, discounts and free lessons</h4>

            <form @click.prevent class="formulario">
                <input type="email" name="email" class="email" placeholder="Enter your email">
                <input type="submit" value="Subscribe" class="btn" data-wait="Please wait...">
            </form>
        </div>

    </section>
</template>

<style scoped>

.newsletter {
    display: flex;
    flex-direction: column;
}

.baixar {
    display: flex;
    flex-direction: column;
    gap: 0.6rem;
    text-align: center;
    padding: 7.65rem 1rem 11.4rem 1rem;
    background: url(../../public/img/wavy-bg.svg) center / cover, linear-gradient(135deg, #fc0a7e, #602bb6);

    @media (min-width: 768px) {
        padding: 6.4rem 0 8.9rem 0;
    }
}   

.baixarTitulo, .contatoTitulo {
    font-size: 1.75rem;
    color: #fff;
    margin: 1.25rem 0;
}

.baixarBtnBox {
    display: flex;
    flex-direction: column;
    gap: .5rem;

    button, a {
        color: #fff;
        font-weight: bold;
        font-size: 1rem;
        padding: 1.25rem 2.5rem;
        background-color: transparent;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        text-decoration: none;
    }

    @media (min-width: 768px) {
        flex-direction: row;
        justify-content: center;
        align-items: center;
    }
}

.baixarBtnBox button:first-child {
    background-color: #fc0a7e;
    transition: bic-bezier(.789, .159, .25, 1);
    transition: background-color 500ms cubic-bezier(.789, .159, .25, 1), color 200ms cubic-bezier(.789, .159, .25, 1);

    &:hover {
        background-color: #fff;
        color: #6b6b6b;
    }
}

.baixarBtnBox a:last-child {
    box-shadow: inset 0 0 0 2px #ffffff33;

    &:hover {
        box-shadow: inset 0 0 0 2px #fff;

    }
}

.contato {
    background-color: #1b1b1b;
    padding: 4.7rem 1rem 6rem;
    display: flex;
    flex-direction: column;
    text-align: center;
}

.contatoSubtitulo {
    color: #6b6b6b;
    font-size: 1rem;
    font-weight: 500;
    line-height: 1.8rem;
    margin-bottom: .6rem;
}

.formulario {
    display: flex;
    flex-direction: column;
    margin-top: 2rem;

    @media (min-width: 768px) {
        flex-direction: row;
        justify-content: center;
    }
}

.email {
    border: none;
    outline: none;
    padding: 1.25rem 2.5rem;
    text-align: center;
    border-top-right-radius: 3px;
    border-top-left-radius: 3px;
    transition: all .5s ease;

    &:focus, &:hover {
        box-shadow: inset 0 0 0 2px #fc0a7e;    
    }

    @media (min-width: 768px)  {
        border-top-left-radius: 3px;
        border-bottom-left-radius: 3px;
        text-align: start;
        padding: 0.6rem 0 0.5rem 1.25rem;
        width: 15rem;
    }
}

.btn {
    border: none;
    padding: 1.25rem 2.5rem;
    background-color: #fc0a7e;
    color: #fff;
    font-size: 1rem;
    font-weight: 600;
    border-bottom-right-radius: 3px;
    border-bottom-left-radius: 3px;
    transition: all 0.5s ease;
    
    @media (min-width: 768px) {
        border-top-right-radius: 3px;
        border-bottom-right-radius: 3px;
    }

    &:hover {
        background-color: #000;
    }
}
</style>