<script></script>

<template>
    <footer class="rodape">
        <img src="../../public/img/icon-footer.png" alt="" class="imgR">

        <nav class="navegation">
            <ul class="lista">
                <li class="item"><a href="#">Email</a></li>
                <li class="item"><a href="#">Instagram</a></li>
                <li class="item"><a href="#">Facebook</a></li>
                <li class="item"><a href="#">Twitter</a></li>
                <li class="item"><a href="#">Image License Info</a></li>
                <li class="item"><a href="#">Powered by Webflow</a></li>
            </ul>
        </nav>
    </footer>
</template>

<style scoped>
.rodape {
    background-color: var(--cinza1);
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 1.9rem 1rem 2.5rem;
}

.imgR {
    width: 136px;
}

.navegation {
    padding: 30px 0;
}

.lista {
    list-style: none;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.item {
    margin: 0 0.9rem 0.75rem;
    font-size: 0.75rem;

    a {
        text-decoration: none;
        color: var(--cinza4);

        &:hover {
            color: var(--branco);
        }
    }
}

</style>