<template>
  <div class="app">
    <Vehicles :vehicles="vehicles" />
  </div>
</template>

<script>
import Vehicles from "./components/Vehicles";

export default {
  name: "App",
  components: {
    Vehicles,
  },
  data() {
    return {
      vehicles: [],
    };
  },
  created() {
    this.vehicles = [
      {
        id: 1,
        title: "SEDANS",
        text: "Choose a sedan for its affordability and excellent fuel economy. Idea for cruising in the city or on your next road trip.",
        img: 'icon-sedans.svg',
      },
      {
        id: 2,
        title: "SUVS",
        text: "Take an SUV for its spacious interior, power and versatility. perfect for your next family vacation and off-road adventures.",
        img: "icon-suvs.svg",
      },
      {
        id: 3,
        title: "LUXURY",
        text: "Cruise in the best car brands without the bloated prices. Enjoy the enhanced comfort of a luxury rental and arrive in style.",
        img: "icon-luxury.svg",
      },
    ];
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@700&family=Lexend+Deca&display=swap");
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
.app {
  max-width: 1125px;
  min-height: 500px;
  border-radius: 10px;
  display: flex;
  width: 80%;
  margin: 4em auto;
  overflow: auto;
  color: hsl(0, 0%, 95%);
}
p {
  color: hsla(0, 0%, 100%, 0.75)
}
</style>
