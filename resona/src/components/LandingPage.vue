<script setup></script>

<template>

    <body class="app-container">
        <header>
            <img></img>
            <nav>
                <img></img>
            </nav>
        </header>
        <div class="title">
            <h1 class="rubik">Resona</h1>
            <h3 class="lexend"> Immersive, Audio-Reactive Experience</h3>
        </div>
        <div class="mission">
            <h3 class="rubik">Our mission</h3>
            <p class="lexend">Resona creates immersive, audio-reactive visuals and media that transform sound into
                real-time
                experiences.
                We help events elevate their energy, engage audiences, and bring music to life through interactive
                technology and design.</p>
        </div>
        <div class="vision">
            <h3 class="rubik">Our vision</h3>
            <p class="lexend">To redefine how people experience sound by becoming the global standard for audio-reactive
                environments,
                where every beat, frequency, and signal shapes a living, responsive world.</p>
        </div>
    </body>

</template>

<style lang="scss" scoped>
.title {
    grid-column: span 2;
    text-align: center;
}

.title h3 {
    font-weight: 800;
    color: #8C030E;
}

.mission {
    grid-column: span 2;
    text-align: center;
    background-color: #260104;
    color: white;
}

.vision {
    grid-column: span 2;
    text-align: center;
    background-color: #40010D;
    color: white;
}
</style>
