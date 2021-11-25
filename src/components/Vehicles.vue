<template>
  <div :key="vehicle.id" v-for="vehicle in vehicles">
    <Vehicle :vehicle="vehicle" />
  </div>
</template>

<script>
import Vehicle from "./Vehicle";

export default {
  name: "Vehicles",
  props: {
    vehicles: Array,
  },
  components: {
    Vehicle,
  },
};
</script>
