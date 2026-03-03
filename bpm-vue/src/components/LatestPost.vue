<script setup></script>

<template>
<main class="app-container">
    <h1>Latest Post</h1>
    <div class="img-container">
        <video src="../assets/instapost.mp4" autoplay muted loop></video>
    </div>
</main>
</template>

<style scoped>
.app-container {
    h1 {
        grid-column: span 2;
        text-align: center;
    }

    .img-container {
        display: grid;
        grid-column: span 2;
        grid-row: span 4;
        margin: 0 auto;
        height: 100%;

        video {
            width: 100%;
            height: 600px;
            object-fit: contain;
        }
    }
}

@media screen and (min-width: 1080px) {
    .app-container {
        h1, .img-container {
            grid-column: span 5;
        }
    }
}
</style>