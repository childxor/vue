<template>
  <div class="hello">
    <h1 v-if="msg != 10 ? false : true">{{ msg }}</h1>
    <h2>{{ msg }}</h2>
    <h2>{{ msg }}</h2>
    <h2>{{ msg }}</h2>
    <h2>{{ as }}</h2>
    <!-- <button v-on:click="Plus()">click</button> -->
    <input v-model="msg" /> <br />
    <a v-bind:href="msg">123</a>
    <button @click="goToAbout">GO TO ABOUT</button>
  </div>
</template>

<script lang="ts">
export default {
  name: "hello world",
  data() {
    return {
      msg: "",
      subTitle: "world",
      as: "goal",
    };
  },
  methods: {
    Plus: function() {
      return this.msg;
    },
    goToAbout() {
      this.$router.push({ name: "About" });
    },
  },
};
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
