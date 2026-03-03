<script setup></script>

<template>

  <body class="app-container">
    <header>
        <h3 class="rubik">portfolio</h3>
    </header>
    <div>
        <video width="300px"><source src="../assets/Motion Concept 1.mp4" type="video/mp4"></video>
        <figcaption class="lexend">description</figcaption>
    </div>
    <div>
        <video width="300px"><source src="../assets/Motion Concept 2.mp4" type="video/mp4"></video>
        <figcaption class="lexend">description</figcaption>
    </div>
    <div>
        <video src=""></video>
        <figcaption class="lexend">description</figcaption>
    </div>
     <div>
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
    border-radius: 20px;
    border: 5px solid #8F0410;
}
</style>
