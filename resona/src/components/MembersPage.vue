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
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
    </div>
    <div class="carousel-nav">
        <button class="lexend"><</button>
        <button class="lexend">></button>
    </div>
  </body>

</template>

<style lang="scss" scoped>
.app-container {
    height: auto;
    grid-template-rows: 1fr;
}

div {
    grid-column: span 2;
    text-align: center;
    justify-items: center;
}

#name {
  background-color: #260104;
  border-radius: 20px;
  color: white;
   width: 300px;
  height: 100px;
}

#role {
  background-color: #8F0410;
  border-radius: 20px;
  color: white;
  width: 300px;
  height: 100px;
}

p {
    padding: 10px;
}

.carousel-nav button {
    border-radius: 20px;
    padding: 5px;
    background: radial-gradient(#D21436, #8C030E, #D21436);
    color: white;
    margin-bottom: 20px;
}
</style>
