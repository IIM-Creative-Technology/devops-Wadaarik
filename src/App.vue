<template>
  <div id="app">
    <firstpage></firstpage>
    <Header></Header>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Firstpage from "./components/firstpage";
import Header from "./components/Header";

export default {
  name: 'App',
  components: {
    Firstpage,
    Header
  }
}
</script>

<style>
  @import url(https://fonts.googleapis.com/css?family=Roboto:400,700);

  @font-face {
    font-family: ArialBlack;
    src: url('../src/assets/arial-black.ttf');
  }
</style>
