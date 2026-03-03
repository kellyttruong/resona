<script setup></script>

<template>
<main class="app-container">
    <section class="links glass">
        <p>Lineup</p>
        <p>Location</p>
        <p>Powered by Resona</p>
    </section>
    <div class="img-container">
        <img src="../assets/white.png" alt="">
    </div>
    <section class="copyright">
        <h2 class="bruno">Base Pulse Music</h2>
        <p>© BPM 2026, all rights reserved.</p>
    </section>
</main>
</template>

<style lang="scss" scoped>
.app-container {
    height: auto;
    grid-template-rows: repeat(4, minmax(0, 1fr));
    background: linear-gradient(90deg, var(--blue), var(--purple));

    .links {
        grid-column: span 2;
        text-align: right;
    }
    .img-container {
        grid-column: span 2;
        grid-row: span 2;
    }
    .copyright {
        grid-column: span 2;
        margin: 0 auto;
        text-align: center;
    }
}

@media (min-width: 1080px) {
    .app-container {
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: repeat(2, minmax(0, 1fr));
        height: auto;

        .img-container {
            grid-column: 1 / span 2;
            grid-row: 1 / span 1;

            img {
                width: 20rem;
            }
        }
        .copyright {
            grid-column: span 4;
            align-self: end;
        }
    }
}
</style>