<script setup></script>

<template>

  <body class="app-container">
    <header>
        <h3 class="rubik">members</h3>
    </header>
    <div class="carousel-track">
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and codin</p>
          </span>
        </div>
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

#role {
  background-color: #8F0410;
  border-radius: 20px;
  color: white;
}
</style>
