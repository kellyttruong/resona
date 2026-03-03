<script setup>
// import { ref, onMounted } from "vue"

// const inner = ref([])
// const current = ref(0)

// function updateCarousel() {
// inner.value.forEach(inner => {
// inner.classList.remove("active", "layer-1", "layer-2", "layer-3")
// })

// const total = inner.value.length

// if (!total) return

// inner.value[current.value]?.classList.add("active")
// inner.value[(current.value + 1) % total]?.classList.add("layer-1")
// inner.value[(current.value + 2) % total]?.classList.add("layer-2")
// inner.value[(current.value + 3) % total]?.classList.add("layer-3")
// }

// function next() {
// current.value = (current.value + 1) % inner.value.length
// updateCarousel()
// }

// function prev() {
// current.value =
// (current.value - 1 + inner.value.length) % inner.value.length
// updateCarousel()
// }

// onMounted(() => {
// inner.value = document.querySelectorAll(".inner")
// updateCarousel()
// }) 
</script>

<template>

  <body class="app-container">
    <header>
        <h3 class="rubik">members</h3>
    </header>
    <div class="carousel">
        <div class="inner">
          <p id="name" class="lexend">Rafsun</p>
          <p id="role" class="lexend">Touch Designer</p>
          <span>
            <p id="task" class="lexend">Stage Visuals, Wayfinding and Ticketing Strategy</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Tyler</p>
          <p id="role" class="lexend">Web Designer, Coder, Visual Creator</p>
          <span>
            <p id="task" class="lexend">BPM Web Design and Coding, Crowd Live Visualizer </p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ann</p>
          <p id="role" class="lexend">Graphic Designer, Video Editor</p>
          <span>
            <p id="task" class="lexend">BPM poster, Presentation Vid</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Remi</p>
          <p id="role" class="lexend">Social Media Spokesperson, Video Editor</p>
          <span>
            <p id="task" class="lexend">Insta Post, Presentation Vid</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Kaisen</p>
          <p id="role" class="lexend">Graphic Designer</p>
          <span>
            <p id="task" class="lexend">Resona logo</p>
          </span>
        </div>
        <div class="inner">
          <p id="name" class="lexend">Ibrahim</p>
          <p id="role" class="lexend">Touch Designer</p>
          <span>
            <p id="task" class="lexend">Live Visuals</p>
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
            <p id="task" class="lexend">Resona Web Design and Coding</p>
          </span>
        </div>
    </div>
    <div class="carousel-nav">
        <button class="lexend" @click="prev"><</button>
        <button class="lexend" @click="next">></button>
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

// .carousel {
//   position: relative;
// }

// .inner {
//   position: absolute;
// }

// .active {
//   transform: translateX(0) scale(1);
//   z-index: 4;
//   opacity: 1;
// }

// .layer-1 {
//   transform: translateX(-25px) scale(0.96);
//   z-index: 3;
//   opacity: 1;
// }

// .layer-2 {
//   transform: translateX(-50px) scale(0.92);
//   z-index: 2;
//   opacity: 1;
// }

// .layer-3 {
//   transform: translateX(-75px) scale(0.88);
//   z-index: 1;
//   opacity: 1;
// }

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
