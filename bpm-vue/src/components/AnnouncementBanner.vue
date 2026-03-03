<script setup></script>

<template>
  <main class="app-container">
    <section class="banner">
      <h1 class="bruno">Don't miss out!</h1>
      <p>Subscribe to our newsletter for updates and exclusive offers.</p>
      <button>Subscribe</button>
    </section>
  </main>
</template>

<style scoped lang="scss">
.app-container {
  height: auto;
  grid-template-rows: repeat(3, minmax(0, 1fr));
  .banner {
    display: grid;
    gap: 20px;
    justify-items: center;
    grid-row: span 2;
    grid-column: span 2;
    background: linear-gradient(180deg, var(--cyan), var(--purple));
    border-radius: 20px;
    padding: 1em;

    h1 {
      text-align: center;
    }
    p {
      width: 100%;
      margin: 0 auto;
    }
  }
}
@media (min-width: 1080px) {
  .app-container {
    .banner {
      border-radius: 0;
      grid-column: span 5;
      grid-template-columns: 1fr 1fr;

      button {
        grid-column: 2;
        grid-row: 1 / span 2;
        align-self: center;
        transform: scale(2);
      }
      h1 {
        justify-self: left;
      }
      p {
        grid-column: 1;
      }
    }
  }
}
</style>
