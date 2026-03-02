<script setup></script>

<template>

  <body>
    <header>
        <h3 class="rubik">members</h3>
    </header>
    <div class="carousel-track">
        <button>
          <p id="name" class="lexend">name</p>
          <p id="description" class="lexend">description</p>
        </button>
    </div>
    <div class="carousel-nav">
        <button><</button>
        <button>></button>
    </div>
  </body>

</template>

<style lang="scss" scoped>
div {
    grid-column: span 2;
    text-align: center;
    margin-top: 30px;
}

#name {
  background-color: #260104;
  border-radius: 20px;
  color: white;
}

#description {
  background-color: #8F0410;
  border-radius: 20px;
  color: white;
}
</style>
