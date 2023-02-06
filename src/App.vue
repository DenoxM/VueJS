<template>
  <div id="app">
    <!--<HelloWorld msg="Hello Vue in CodeSandbox!" /> -->
    <p>Liste des emojis:</p>
    <Test v-for="post in posts" :key="post" :msg="post.emoji" />
  </div>
</template>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<script>
//import HelloWorld from "./components/HelloWorld";
import Test from "./components/Test";

export default {
  name: "App",
  components: {
    Test,
    //HelloWorld
  },
  data() {
    return {
      posts: [{ emoji: ":)" }, { emoji: ">:(" }, { emoji: ":'(" }],
    };
  },
};
</script>