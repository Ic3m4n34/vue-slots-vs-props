<template>
  <div class="hello">
    <button class="button is-primary">I'm a button</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    showIcon: false,
    showButton: false,
  },
  data() {
    return {
      msg: "Hello World"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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
