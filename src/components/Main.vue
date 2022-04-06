<template>
  <main>
    <div id="main-container">
      <div class="content">
        <h2>--- Content goes here ---</h2>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: "mainComponent",
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
