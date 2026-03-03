<script setup></script>

<template>
  <main class="app-container">
    <section class="date">
      <h1>Friday</h1>
      <h6>June 12th</h6>
    </section>
    <section class="headliner">
      <div class="img-container">
        <img src="../assets/fred_again.jpg" alt="Fred Again" />
        <h2 class="name glass">Fred again..</h2>
      </div>
    </section>
    <section class="headliner">
      <div class="img-container">
        <img src="../assets/john_summit.jpg" alt="John Summit" />
        <h2 class="name glass">John Summit</h2>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/rezz.jpg" alt="Rezz" />
        <h6 class="name glass">Rezz</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/virtual_riot.jpg" alt="Virtual Riot" />
        <h6 class="name glass">Virtual Riot</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/disco_lines.jpg" alt="Disco Lines" />
        <h6 class="name glass">Disco Lines</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/dom_dolla.jpg" alt="Dom Dolla" />
        <h6 class="name glass">Dom Dolla</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/lcd_soundsystem.jpg" alt="LCD Soundsystem" />
        <h6 class="name glass">LCD Soundsystem</h6>
      </div>
    </section>
    <section class="date">
      <h1>Saturday</h1>
      <h6>June 13th</h6>
    </section>
    <section class="headliner">
      <div class="img-container">
        <img src="../assets/TheFatRat.jpg" alt="TheFatRat" />
        <h2 class="name glass">TheFatRat</h2>
      </div>
    </section>
    <section class="headliner">
      <div class="img-container">
        <img src="../assets/porter_robinson.webp" alt="Porter Robinson" />
        <h2 class="name glass">Porter Robinson</h2>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/s3rl.jpg" alt="S3RL" />
        <h6 class="name glass">S3RL</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/machine_girl.jpg" alt="Machine Girl" />
        <h6 class="name glass">Machine Girl</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/goreshit.jpg" alt="Goreshit" />
        <h6 class="name glass">Goreshit</h6>
      </div>
    </section>
    <section class="artist">
      <div class="img-container">
        <img src="../assets/ada_rook.jpg" alt="Ada Rook" />
        <h6 class="name glass">Ada Rook</h6>
      </div>
    </section>
  </main>
</template>

<style scoped lang="scss">
.app-container {
  grid-template-rows: auto;
  height: auto;
  .date {
    grid-column: span 2;
    text-align: center;
  }
  .img-container {
    overflow: visible;
    z-index: 1;
    border-radius: 20px;
    img {
      border-radius: 20px;
      z-index: 1;
      aspect-ratio: 16/9;
      object-position: top;
    }
  }
  .headliner {
    grid-column: span 2;
    display: grid;

    .glass {
      padding: 10px;
    }
  }
  .artist {
    display: grid;

    .glass {
      padding: 0;
    }
  }
  .name {
    position: absolute;
    bottom: 0;
    left: 0;
    text-align: center;
    z-index: 100;
    width: 100%;
  }
}

@media (min-width: 1080px) {
  .app-container {
    grid-template-columns: repeat(6, 1fr);
    .date {
      grid-column: span 6;
      padding-top: 10rem;
    }
    .headliner {
      grid-column: span 3;
    }
  }
}
</style>
