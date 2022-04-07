<template>
  <main>
    <div class="jumbotron"></div>
    <div id="main-container">
      <div class="item-container">
        <SerieItem v-for="(item, index) in series" :key="index" :serie="item" />
      </div>
    </div>
  </main>
</template>

<script>
import SerieItem from "@/components/SerieItem.vue";

export default {
  name: "mainComponent",
  props: {
    series: Array,
  },
  components: {
    SerieItem,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
main {
  color: white;
  background: black;

  .jumbotron {
    background-image: url(@/assets/jumbotron.jpg);
    background-size: cover;
    height: 400px;
    max-width: 100vw;
  }

  #main-container {
    width: 80%;
    margin: 0 auto;

    .item-container {
      display: flex;
      flex-wrap: wrap;
    }
  }
}
</style>
