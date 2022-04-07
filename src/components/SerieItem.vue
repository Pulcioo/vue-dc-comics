<template>
  <div class="card">
    <img :src="serie.thumb" alt="cover" />
    <h2>{{ serie.series }}</h2>
  </div>
</template>

<script>
export default {
  name: "seriesItem",
  props: {
    serie: Object,
  },
};
</script>

<style scoped lang="scss">
.card {
  display: flex;
  flex-direction: column;
  max-width: 150px;
  margin: 15px;

  img {
    width: 150px;
    height: 200px;
  }

  h2 {
    font-size: 14px;
    padding-top: 10px;
    text-transform: uppercase;
  }
}
</style>