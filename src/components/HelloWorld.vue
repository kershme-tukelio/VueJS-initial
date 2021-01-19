<template>
  <div class="hello">
    <h1>{{ msg ? "msg je true" : "msg je false" }}</h1>
    <h2>{{ typeof noviProp }}</h2>
    <div v-bind:id="noviProp">
      Ovaj div ima id {{ msg.split(' ').reverse().join(' ')}}
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
    noviProp: String
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
