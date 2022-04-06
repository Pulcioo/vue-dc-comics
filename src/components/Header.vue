<template>
  <header>
    <div id="header-container">
      <img src="../assets/dc-logo.png" alt="Logo" />
      <div class="header-menu">
        <ul>
          <li>
            <a href="#"> <strong>CHARACTERS</strong> </a>
          </li>
          <li>
            <a href="#"><strong> COMICS</strong></a>
          </li>
          <li>
            <a href="#"><strong> MOVIES</strong></a>
          </li>
          <li>
            <a href="#"><strong> TV</strong></a>
          </li>
          <li>
            <a href="#"><strong> GAMES</strong></a>
          </li>
          <li>
            <a href="#"><strong>COLLECTIBLES</strong> </a>
          </li>
          <li>
            <a href="#"><strong>VIDEOS</strong> </a>
          </li>
          <li>
            <a href="#"><strong>FANS</strong> </a>
          </li>
          <li>
            <a href="#"><strong>NEWS</strong> </a>
          </li>
          <li>
            <a href="#"><strong>SHOP</strong> </a>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "headerComponent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#header-container {
  width: 80%;
  margin: 15px auto;
  display: flex;
  justify-content: space-between;

  img {
    width: 80px;
  }

  .header-menu {
    display: flex;
    align-items: center;

    ul {
      display: flex;

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
