<template>
  <div>
    <button @click="incre">+</button>
    <button v-on:click="decre">-</button>
    <p>{{num}}</p>
  </div>
</template>

<script>
export default {
  props: ['num'],
  data () {
    return {

    }
  },
  methods: {
    incre () {
      this.$emit('incre')
    },
    decre () {
      this.$emit('decre')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
