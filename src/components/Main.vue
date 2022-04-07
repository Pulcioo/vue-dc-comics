<template>
  <main>
    <div class="jumbotron">
      <button type="button"><h3>CURRENT SERIES</h3></button>
    </div>
    <div id="main-container">
      <div class="item-container">
        <SerieItem v-for="(item, index) in series" :key="index" :serie="item" />
      </div>
      <div class="load-more-button">
        <button type="button">
          <span><strong>LOAD MORE</strong></span>
        </button>
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
    position: relative;
    margin-bottom: 25px;

    button {
      padding: 10px;
      margin-bottom: 5px;
      background: #008dff;
      color: white;
      border: none;
      position: absolute;
      bottom: -20px;
      left: 150px;
    }
  }

  #main-container {
    width: 80%;
    margin: 0 auto;

    .item-container {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }

    .load-more-button {
      width: 100%;
      display: flex;
      justify-content: center;
      padding-bottom: 10px;

      button {
        padding: 10px;
        margin-bottom: 5px;
        background: #008dff;
        color: white;
        border: none;
      }
    }
  }
}
</style>
