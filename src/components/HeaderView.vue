<script>
    import logo from '../../public/img/logo-richard.png'
    export default {
        data() {
            return {
                logoImg: logo,
                toggleMenu: false
            }
        },
        methods: {
            menu() {
                this.toggleMenu = !this.toggleMenu
            },
            redirect() {
                window.open('https://momentum-template.webflow.io/', '_blanck')
            }
        }
    }
</script>

<template>
    <header id="header">
        <div class="cabecalho">
            <img :src="logoImg" alt="Logo Richard" class="logo" @click="redirect">
    
            <nav class="navegation">
                <ul class="lista">
                    <li><a href="#about">About</a></li>
                    <li><a href="#features">Features</a></li>
                    <li><a href="#how-to-use">How to use</a></li>
                    <li><a href="#download">Download</a></li>
                </ul>
    
                <div :class="['btn', {'btnPreto' : toggleMenu}]" @click="menu">
                    <button>Menu</button>
                </div>
            </nav>
        </div>

        <div :class="['menuMob', {'menuOpen' : toggleMenu}]">
            <ul class="listaMob">
                <li><a href="#about">About</a></li>
                <li><a href="#features">Features</a></li>
                <li><a href="#how-to-use">How to use</a></li>
                <li><a href="#download">Download</a></li>
            </ul>
        </div>
    </header>

    <div class="btnVoltar">
        <a href="#header">Voltar</a>
    </div>
</template>

<style scoped>
header {
    display: flex;
    flex-direction: column;
    position: absolute;
    right: 0;
    left: 0;
}

.cabecalho {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 6vh;
    background-color: transparent;
    padding: 2rem 0 2rem 1rem;

    @media (min-width: 992px) {
        padding: 3rem 8rem;
    }
}

.logo {
    width: 120px;
    height: 43px;
}

.lista {
    display: none;
    @media (min-width: 992px) {
        display: flex;
        gap: 3rem;
        list-style: none;

        li a {
            text-decoration: none;
            color: #fff;
            padding-bottom: .8rem;

            &:hover {
            border-bottom: 4px solid #dd1173;
        }
        }
    }
}

.btn {
    height: calc(6vh + 2rem);
    width: 20vw;
    display: flex;
    justify-content: center;
    align-items: center;

    @media (min-width: 992px) {
        display: none;
    }

}

.btnPreto {
    background-color: #000;
}

.menuMob {
    background-color: #000;
    height: 0;
    overflow: hidden;
    transition: all .5s ease;

    @media (min-width: 992px) {
        display: none;
    }
}

.menuOpen {
    height: 20rem;
    transition: all .5s ease;
}

.listaMob {
    display: flex;
    flex-direction: column;
    gap: 3.5rem;
    padding: 2.5rem 2rem;
    font-size: 1.1rem;

    li a {
        color: #fff;
        text-decoration: none;
    }

}

.btnVoltar {
    padding: 1rem 1.5rem;
    background-color: #000;
    position: fixed;
    bottom: 1rem;
    right: 1rem;
    box-shadow: inset 0 0 0 2px #dd1173;
    border-radius: 5px;

    a {
        text-decoration: none;
        color: #fff;
        font-weight: bold;
    }
}

</style>