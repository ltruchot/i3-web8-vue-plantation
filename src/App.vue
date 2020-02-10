<template>
  <div>
    <PlantList />
  </div>
</template>

<script>
import PlantList from './components/PlantList.vue'

export default {
  name: 'App',
  components: {
    PlantList
  },
  data: function () {
    return {
      salutation: "Coucou les Web8"
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
