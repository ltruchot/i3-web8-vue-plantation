<template>
    <li>
        {{plant.name}}
        <button @click="arroser" v-if="!plant.arr">Arroser</button>
    </li>
</template>

<script>
export default {
  name: 'Plant',
  props: {
      plant: Object
  },
  methods: {
      arroser () {
          this.plant.arr = true;
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
