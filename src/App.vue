<template>
  <div>
    <h1>{{ title }}</h1>
    <ninjas></ninjas>
    {{ someData }}

    <hr>
    <button @click="add">Click me</button>
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
  methods: {
    add: function(){
      console.log('Metallica');
    }

  }
};
</script>

<style>
h1 {
  color: purple;
}
</style>
