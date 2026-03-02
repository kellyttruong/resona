<script setup></script>

<template>
  
   <body class="app-container">
    <header>
        <h3 class="rubik">partners</h3>
    </header>
    <div class="mmi">
        <a href="https://582multi.media/"><img src="../assets/symbol_582_w.png" alt id="mlo"></a>
    </div>
    <div class="bpm">
        <a href=""><img src="../assets/white.png" alt id="blo"></a>
    </div>
   </body>

</template>

<style lang="scss" scoped>
div {
    grid-column: span 2;
    text-align: center;
    margin-top: 30px;
}

div:hover img {
    transform: scale(1.08);
}

#mlo {
    width: 200px;
}

#blo {
    width: 400px;
}
</style>
