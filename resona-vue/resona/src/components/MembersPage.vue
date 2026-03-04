<script setup>
import { ref, computed } from "vue";

const members = [
  { name: "Rafsun", role: "Touch Designer", task: "Stage Visuals, Wayfinding and Ticketing Strategy" },
  { name: "Tyler", role: "Web Designer, Coder, Visual Creator", task: "BPM Web Design and Coding, Crowd Live Visualizer" },
  { name: "Ann", role: "Graphic Designer, Video Editor", task: "BPM poster, Presentation Vid" },
  { name: "Remi", role: "Social Media, Video Editor", task: "Insta Post, Presentation Vid" },
  { name: "Kaisen", role: "Graphic Designer", task: "Resona logo" },
  { name: "Ibrahim", role: "Touch Designer", task: "Live Visuals" },
  { name: "Kelly", role: "Graphic Designer, Coder", task: "BPM logo, Resona Website" },
  { name: "Ray", role: "Web Designer, Coder", task: "Resona Web Design and Coding" }
];

const currentIndex = ref(0);
const currentMember = computed(() => members[currentIndex.value]);

const next = () => {
  currentIndex.value = (currentIndex.value + 1) % members.length;
};

const prev = () => {
  currentIndex.value = (currentIndex.value - 1 + members.length) % members.length;
};
</script>

<template>
  <div class="app-container">
    <header>
      <h3 class="rubik">members</h3>
    </header>

    <div class="carousel">
      <div class="inner">
        <p class="name lexend">{{ currentMember.name }}</p>
        <p class="role lexend">{{ currentMember.role }}</p>
        <p class="task lexend">{{ currentMember.task }}</p>
      </div>
    </div>

    <div class="carousel-nav">
      <button class="lexend" id="prev" @click="prev"><</button>
      <button class="lexend" id="next" @click="next">></button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.app-container {
  height: auto;
  display: grid;
  justify-items: center;
  margin-bottom: 30px;
}

.carousel {
  display: grid;
  grid-column: span 2;
  place-items: center;
  margin: 30px 0;
}

.inner {
  display: grid;
  gap: 20px;
  justify-items: center;
}

.name,
.role {
  display: grid;
  place-items: center;
  border-radius: 20px;
  color: white;
  width: 300px;
  height: 100px;
}

.name {
  background-color: #260104;
}

.role {
  background-color: #8F0410;
}

.task {
  color: white;
  text-align: center;
  max-width: 400px;
}

.carousel-nav {
  display: grid;
  grid-auto-flow: column;
  grid-row: 4;
  grid-column: span 2;
  gap: 20px;
}

.carousel-nav button {
  height: max-content;
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

  justify-self: center;
  width: 50px;
}


@media screen and (min-width: 1080px) {
  .carousel, .carousel-nav {
    grid-column: 2 / span 3;
  }
  .carousel {
    grid-row: 2;
  }
  .carousel-nav {
    grid-row: 3;
    justify-items: right;
  }
  header {
    position: absolute;
    right: 0;
  }
}
</style>