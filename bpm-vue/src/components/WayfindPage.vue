<script setup></script>

<template>
  <main class="app-container">
    <h1>Location</h1>
    <div class="embed-map-fixed">
      <div class="embed-map-container"><iframe class="embed-map-frame" frameborder="0" scrolling="no" marginheight="0"
          marginwidth="0"
          src="https://maps.google.com/maps?width=600&height=400&hl=en&q=parc%20jean%20drapeau&t=&z=14&ie=UTF8&iwloc=B&output=embed"></iframe>
      </div>
    </div>
    <h2>1, circuit Gilles Villeneuve, Montréal, QC H3C 1A9, Canada</h2>
  </main>
</template>

<style scoped lang="scss">
.app-container {
  h1 {
    margin: 0 auto;
    grid-column: span 2;
  }
  .embed-map-fixed {
    position: relative;
    text-align: right;
    width: 100%;
    height: 100%;
    margin: 0 auto;
    grid-column: span 2;
    grid-row: span 2;
  }

  .embed-map-container {
    overflow: hidden;
    background: none !important;
    width: 100%;
    height: 100%;
  }

  .embed-map-frame {
    width: 100%;
    height: 100%;
  }
  
  h2 {
    grid-column: span 2;
    text-align: center;
  }
}

@media screen and (min-width: 1080px) {
  .app-container {
    h1 {
      grid-column: span 5;
    }

    .embed-map-fixed {
      grid-column: span 3;
      grid-row: span 5;
    }

    h2 {
      grid-column: span 2;
      grid-row: span 3;
      align-self: center;
      text-align: right;
    }
  }

}
</style>