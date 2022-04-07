<template>
  <div id="app">
    <Header :links="menuItem" />
    <Main />
    <Info />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Info from "./components/Info.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  data() {
    return {
      menuItem: [
        { message: "CHARACTER" },
        { message: "COMICS" },
        { message: "MOVIES" },
        { message: "TV" },
        { message: "GAMES" },
        { message: "COLLECTIBLES" },
        { message: "VIDEOS" },
        { message: "FANS" },
        { message: "NEWS" },
        { message: "SHOP" },
      ],
    };
  },
  components: {
    Header,
    Main,
    Info,
    Footer,
  },
};
</script>

<style lang="scss">
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
