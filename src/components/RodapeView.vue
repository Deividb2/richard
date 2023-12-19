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
    background-color: #1b1b1b;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 30px 16px 40px;
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
    margin: 0 15px 12px;
    font-size: 12px;

    a {
        text-decoration: none;
        color: #6b6b6b;
    }
}

</style>