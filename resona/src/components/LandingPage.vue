<script setup></script>

<template>

    <body class="app-container">
        <img src="../assets/Artboard 1.png" alt id="logo">
        <header class="navi">
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
    grid-template-rows: 1fr;
    margin-bottom: 30px;
}

#logo {
    grid-column: 1;
    grid-row: 1;
    width: 200px;
}

#ham-menu {
    width: 40px;
    grid-column: 2;
    margin-top: 25px;
}

.title {
    grid-column: span 2;
    text-align: center;
    margin-bottom: 50px;
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
    padding: 8px;
}

.vision {
    grid-column: span 2;
    text-align: center;
    background-color: #40010D;
    margin-left: 10px;
    margin-right: 10px;
    border-radius: 20px;
    padding: 8px;
}

.mission h3,
.vision h3 {
    color: white;
    margin-top: 10px;
}

.mission p,
.vision p {
    color: white;
    margin-top: 10px;
    padding: 10px;
}

@media screen and (min-width: 1080px) {
    .app-container {
        grid-template-columns: repeat(4, 1fr);
    }
    .title {
        grid-column: span 5;
    }
    .title h1 {
        font-size: 100px;
    }
    .title h3 {
        font-size: 40px;
    }
    .navi {
        grid-column: 5;
        justify-self: right;
    }
    #logo {
        width: 300px;
    }
    .mission {
        grid-column: 2;
    }
    .vision {
        grid-column: 3;
    }
    .mission h3, .vision h3 {
        font-size: 30px;
    }
    .mission p, .vision p {
        font-size: 15px;
    }
}
</style>
