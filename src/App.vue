<template>
  <Navbar />
  <Header></Header>
  <Relasi />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Header from "./components/Header.vue";
import Relasi from "./components/Relasi.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Header,
    Relasi,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0;
}
</style>
