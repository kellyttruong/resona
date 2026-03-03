<script setup>
import { ref, computed } from 'vue'

const isOpen = ref(false)

const toggleMenu = () => {
  isOpen.value = !isOpen.value
}

const closeMenu = () => {
  isOpen.value = false
}
</script>

<template>
  <nav :class="{ open: isOpen }">
    <div class="top">
      <div class="img-container">
        <img src="../assets/white.png" alt="" />
      </div>

      <h2>2026</h2>

      <button class="hamburger" @click="toggleMenu">
        <div class="line"></div>
        <div class="line"></div>
        <div class="line"></div>
      </button>
    </div>

    <div class="links">
      <a href="#home" @click="closeMenu">Home</a>
      <a href="#lineup" @click="closeMenu">Lineup</a>
      <a href="https://resona.capython.com/">Powered by Resona</a>
    </div>
  </nav>
</template>

<style scoped lang="scss">
nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100px;
  background: linear-gradient(90deg, var(--blue), var(--purple));
  z-index: 101;
  transition: 0.3s ease;

  .top {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    align-items: center;
    padding: 0 1rem;
    height: 100px;
  }

  .img-container {
    justify-self: start;
  }

  h2 {
    text-align: center;
    color: white;
  }

  .hamburger {
    display: grid;
    justify-self: end;
    background: none;
    border: none;
    cursor: pointer;

    .line {
      height: 2px;
      width: 1.5em;
      background-color: white;
      margin-bottom: 4px;
      transition: 0.3s;
    }
  }

  /* LINKS (hidden by default on mobile) */
  .links {
    position: fixed;
    inset: 0;
    background: linear-gradient(180deg, var(--blue), var(--purple));
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 2rem;

    transform: translateY(-100%);
    transition: 0.3s ease;

    a {
      color: white;
      text-decoration: none;
      font-size: 2rem;
    }
  }

  &.open {
    .links {
      transform: translateY(0);
    }
  }
}

@media (min-width: 1080px) { nav { width: 100%; .img-container { img { width: 100px; margin: 0; } } } }
</style>