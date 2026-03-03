<script setup></script>

<template>

  <body class="app-container">
    <header>
        <h3 class="rubik">portfolio</h3>
    </header>
    <div class="left">
        <video src="../assets/Motion Concept 1.mp4" controls poster>motion concept 1</video>
        <figcaption class="lexend">description</figcaption>
    </div>
    <div class="right">
        <video src="../assets/Motion Concept 2.mp4" controls poster>motion concept 1</video>
        <figcaption class="lexend">description</figcaption>
    </div>
    <div class="left">
        <video src=""></video>
        <figcaption class="lexend">description</figcaption>
    </div>
     <div class="right">
        <video src=""></video>
        <figcaption class="lexend">description</figcaption>
    </div>
  </body>

</template>

<style lang="scss" scoped>
.app-container {
    height: auto;
    grid-template-rows: 1fr;
    margin-bottom: 30px;
}
div {
    grid-column: span 2;
    text-align: center;
}

figcaption {
    color: white;
}

video {
  width: 300px;

  background: #8F0410;
  border: 5px solid transparent;
  border-radius: 20px;
  cursor: pointer;

  background-image: 
  linear-gradient(#8f0410, #8F0410),
  radial-gradient(#D21436, #8C030E, #D21436);

  background-origin: border-box;
  background-clip: padding-box, border-box;

  box-shadow: 0 0 12px rgba(143, 4, 16);
}

@media screen and (min-width: 1080px) {
    .app-container {
        gap: 5rem;
    }
    video {
        width: 500px;
    }
    .left {
        grid-column: 2 / span 2;
    }
    .right {
        grid-column: 3 / span 2;
    }
    .right video{
        grid-column: 2;
    }
    .left, .right{
        display: grid;
        grid-template-columns: 1fr 1fr;
        align-items: center;
    }
   .right figcaption {
        grid-column: 1;
        grid-row: 1;
    }
}
</style>
