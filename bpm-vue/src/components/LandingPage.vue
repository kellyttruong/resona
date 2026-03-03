<script setup></script>

<template>
  <main class="app-container">
    <div class="img-container logo">
      <img src="../assets/white.png" alt="" />
    </div>
    <section class="info glass">
      <p>Friday June 12th</p>
      <h3>Fred Again</h3>
      <h3>John Summit</h3>
      <div class="spacer"></div>
      <p>Saturday June 13th</p>
      <h3>TheFatRat</h3>
      <h3>Porter Robinson</h3>
    </section>
    <section class="buttons">
      <button>2026 Tickets</button>
      <button>Full Lineup</button>
    </section>
  </main>
</template>

<style lang="scss" scoped>
.app-container {
  grid-template-rows: auto;
  margin-top: 60px;
  .logo {
    grid-column: span 2;
    grid-row: span 2;
    img {
      height: 100%;
      overflow: visible;
    }
  }
  .info {
    display: grid;
    grid-column: span 2;
    grid-row: span 2;
    text-align: center;

    .spacer {
      height: 2em;
    }
  }
  .buttons {
    display: grid;
    grid-column: span 2;
    grid-row: span 1;
    grid-template-columns: auto auto;
    gap: 1em;
    justify-content: center;
    align-items: center;
  }
}

@media (min-width: 1080px) {
  .app-container {
    grid-template-rows: repeat(5, minmax(0, 1fr));

    .img-container {
      img {
        width: auto;
      }
    }
    .logo {
      grid-column: 2 / span 3;
      grid-row: 1 / span 2;
    }
    .info, .buttons {
      grid-column: 2 / span 3;
    }
  }
}
</style>
