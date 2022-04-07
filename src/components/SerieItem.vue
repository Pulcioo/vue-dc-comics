<template>
  <div class="card">
    <img :src="serie.thumb" />
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
</style>