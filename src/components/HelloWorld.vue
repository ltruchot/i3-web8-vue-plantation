<template>
  <div class="hello">
    <h1 v-on:click="console.log">{{ msg }} {{yo}}</h1>
    {{ titi }}
    {{ take([1, 2, 3, 4], 2) }}

  <h2 v-text="'<span>toto</span> est sympa'"></h2>
  <h2 v-html="'<span>toto</span> est sympa'"></h2>
  <button v-bind:disabled="true">Toto</button>

  </div>
</template>

<script>


import { take } from "lodash";

export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    titi: Number
  },
  data: function() {
    return {
      yo: "yeah !",
      take: take,
      console: console
    };
  },
  methods: {
    onBtnClick () {
      console.log("toto")
    },
    log (e) {
      console.log(e)
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
