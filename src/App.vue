<template>
  <div id="app">
    <v-header></v-header>
    <v-main></v-main>
  </div>
</template>

<script>
import vHeader from "./components/header";
import vMain from "./components/main";
export default {
  components: {
    vHeader,
    vMain
  }
};
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>
