<template>
  <header>
    <div id="header-container">
      <img src="../assets/dc-logo.png" alt="Logo" />
      <div class="header-menu">
        <ul>
          <li v-for="item in links" :key="item.message">
            <a href="#"
              ><strong>{{ item.message }}</strong></a
            >
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "headerComponent",
  props: {
    links: Array,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#header-container {
  width: 80%;
  margin: 15px auto;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;

  img {
    width: 80px;
  }

  .header-menu {
    display: flex;
    align-items: center;

    ul {
      display: flex;
      flex-wrap: wrap;

      li {
        list-style-type: none;

        a {
          text-decoration: none;
          color: black;
          margin: 10px;
          font-size: 14px;

          &:hover {
            color: #0282f9;
          }
        }
      }
    }
  }
}
</style>
