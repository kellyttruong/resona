<script setup>
import { ref } from 'vue'

const isOpen = ref(false)

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}

const closeMenu = () => {
  isOpen.value = false
}
</script>

<template>

    <body class="app-container">
    <img src="../assets/Artboard 1.png" alt="" id="logo" />

    <header class="navi">
      <nav>
        <img
          src="../assets/ham menu 2.png"
          alt=""
          id="ham-menu"
          @click="toggleMenu"
        />
      </nav>
    </header>

    <!-- FULLSCREEN MENU -->
    <div class="fullscreen-menu" :class="{ active: isOpen }">
      <button class="close-btn" @click="closeMenu">✕</button>
      <ul>
        <li><a class="lexend" href="#home" @click="closeMenu">Home</a></li>
        <li><a class="lexend" href="#mission" @click="closeMenu">Our Mission</a></li>
        <li><a class="lexend" href="#vision" @click="closeMenu">Our Vision</a></li>
      </ul>
    </div>

    <div class="title" id="home">
      <h1 class="rubik">Resona</h1>
      <h3 class="lexend">Immersive, Audio-Reactive Experience</h3>
    </div>

    <div class="mission" id="mission">
      <h3 class="rubik">Our mission</h3>
      <p class="lexend">
        Resona creates immersive, audio-reactive visuals and media that
        transform sound into real-time experiences...
      </p>
    </div>

    <div class="vision" id="vision">
      <h3 class="rubik">Our vision</h3>
      <p class="lexend">
        To redefine how people experience sound by becoming the global standard...
      </p>
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
    // margin-top: 25px;
}

.navi {
        position: absolute;
        top: 30px;
  right: 40px;
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
        height: auto;
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
    #logo {
        width: 300px;
    }
    .mission {
        grid-column: 1;
        grid-column: span 2;
        height: 200px;
        margin-left: 30px;
        place-content: center;
    }
    .vision {
        grid-column: 3;
        grid-column: span 2;
        height: 200px;
        place-content: center;
    }
    .mission h3, .vision h3 {
        font-size: 30px;
    }
    .mission p, .vision p {
        font-size: 15px;
    }
}

html {
  scroll-behavior: smooth;
}

/* FULLSCREEN OVERLAY */
.fullscreen-menu {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  background: #260104;
  display: grid;
  justify-content: center;
  align-items: center;
  transform: translateY(-100%);
  transition: transform 0.4s ease;
  z-index: 1000;
}

.fullscreen-menu.active {
  transform: translateY(0);
}

.fullscreen-menu ul {
  list-style: none;
  padding: 0;
  text-align: center;
}

.fullscreen-menu li {
  margin: 30px 0;
}

.fullscreen-menu a {
  color: white;
  text-decoration: none;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
}

.fullscreen-menu a:hover {
  color: #D21436;
}

.close-btn {
  position: absolute;
  top: 30px;
  right: 40px;
  background: none;
  border: none;
  font-size: 40px;
  color: white;
  cursor: pointer;
}
</style>
