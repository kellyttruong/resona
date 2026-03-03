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
        <div class="inner">
          <p id="name" class="lexend">Kelly</p>
          <p id="role" class="lexend">Graphic Designer, Coder</p>
          <span>
            <p id="task" class="lexend">BPM logo, Resona Website</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ray</p>
          <p id="role" class="lexend">Web Designer, Coder</p>
          <span>
            <p id="task" class="lexend">Resona web design and coding</p>
          </span>
        </div>
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
    margin-bottom: 30px;
}

div {
    grid-column: span 2;
    text-align: center;
    justify-items: center;
}

#name {
  display: grid;
  align-items: center;
  background-color: #260104;
  border-radius: 20px;
  color: white;
   width: 300px;
  height: 100px;
}

#role {
  display: grid;
  align-items: center;
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
  padding: 15px;
  font-size: 16px;
  color: white;
  background: #8F0410;
  border: 2px solid transparent;
  border-radius: 20px;
  cursor: pointer;

  background-image: 
    linear-gradient(#8f0410, #8F0410),
    radial-gradient(#D21436, #8C030E, #D21436);

  background-origin: border-box;
  background-clip: padding-box, border-box;

  box-shadow: 0 0 12px rgba(143, 4, 16);
}
</style>
