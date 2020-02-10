<template>
  <ul>
      <Plant v-for="plant in plants" :key="plant.name" :plant="plant" />  
  </ul>
</template>

<script>
import Plant from "./Plant";

export default {
  name: 'PlantList',
  components: {
      Plant
  },
  data: function() {
    return {
        plants: [
            { name: "Succulente", arr: true}, 
            {name: "bonzaï", arr: false}
        ]
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
