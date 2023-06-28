<template>
  <div>
    <h1>{{ title }}</h1>
    <ninjas></ninjas>
    {{ someData }}
  </div>
</template>

<script>
// Imports
import Ninjas from "./Ninjas.vue";

export default {
  data() {
    return {
      title: "Ninja App",
      someData: ["string", true, false, 2, { name: "Marko" }],
    };
  },
  components: {
    ninjas: Ninjas,
  },
};
</script>

<style>
h1 {
  color: purple;
}
</style>
