<template>
  <main>
    <div id="main-container">
      <SerieItem v-for="(item, index) in series" :key="index" :serie="item" />
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

  #main-container {
    width: 80%;
    margin: 0 auto;
  }
}

h2 {
  padding: 40px 0;
}
</style>
