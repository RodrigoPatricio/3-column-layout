<template>
  <div :class="[vehicle.title]">
    <img v-bind:src="require('../assets/' + vehicle.img)" class="img" />
    <h1>{{ vehicle.title }}</h1>
    <p class="description">{{ vehicle.text }}</p>
    <Button />
  </div>
</template>

<script>
import Button from "./Button";

export default {
  name: "Vehicle",
  props: {
    vehicle: Object,
  },
  components: {
    Button,
  },
};
</script>

<style>
.description {
  font-family: Big Shoulders Display;
  font-size: 15px;
  margin-top: 3em;
}
.SEDANS {
  font-family: Lexend Deca;
  background: hsl(31, 77%, 52%);
  height: 100%;
  padding: 50px;
}
.SUVS {
  font-family: Lexend Deca;
  background: hsl(184, 100%, 22%);
  height: 100%;
  padding: 50px;
}
.LUXURY {
  font-family: Lexend Deca;
  background: hsl(179, 100%, 13%);
  height: 100%;
  padding: 50px;
}
.img {
  margin-bottom: 2em;
}
</style>
