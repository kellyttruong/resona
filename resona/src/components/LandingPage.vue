<script setup></script>

<template>

    <body class="app-container">
        <header class="navi">
            <img src="" alt="logo">
            <nav>
                <img src="../assets/ham menu 2.png" alt id="ham-menu">
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
.app-container {
    height: auto;
}

header {
    grid-column: span 2;
    text-align: center;
}

#ham-menu {
    width: 40px;
}

.title {
    grid-column: span 2;
    text-align: center;
}

.title h1 {
    background: -webkit-radial-gradient(#D21436, #8C030E, #D21436);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 80px;
}

.title h3 {
    font-weight: 800;
    color: #8C030E;
    font-size: 20px;
}

.mission {
    grid-column: span 2;
    text-align: center;
    background-color: #260104;
    margin-left: 10px;
    margin-right: 10px;
    border-radius: 20px;
}

.vision {
    grid-column: span 2;
    text-align: center;
    background-color: #40010D;
    margin-left: 10px;
    margin-right: 10px;
    border-radius: 20px;
}

.mission h3,
.vision h3 {
    color: white;
    margin-top: 30px;
}

.mission p,
.vision p {
    color: white;
    margin-top: 10px;
    padding: 10px;
}
</style>
