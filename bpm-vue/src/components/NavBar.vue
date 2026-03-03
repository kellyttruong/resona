<script setup></script>

<template>
    <nav>
        <div class="img-container">
            <img src="../assets/white.png" alt="">
        </div>
        <h2>2026</h2>
        <button class="hamburger">
            <div class="line"></div>
            <div class="line"></div>
            <div class="line"></div>
        </button>
    </nav>
</template>

<style scoped lang="scss">
nav {
    position: fixed;
    top: 0;
    display: grid;
    padding: 0 1rem;
    align-items: center;
    grid-template-columns: 1fr 1fr 1fr;
    height: 100px;
    background: linear-gradient(90deg, var(--blue), var(--purple));
    z-index: 101;

    .img-container {
        justify-self: start;
    }
    h2 {
        text-align: center;
    }
    .hamburger {
        display: grid;
        justify-self: end;

        .line {
            height: 2px;
            width: 1em;
            background-color: white;
            z-index: 10;
            margin-bottom: 2px;
        }
    }
}
@media (min-width: 1080px) {
    nav {
        width: 100%;
        .img-container {
            img {
                width: 100px;
                margin: 0;
            }
        }
    }
}
</style>