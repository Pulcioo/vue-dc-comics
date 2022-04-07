<template>
  <div id="info-container">
    <ul class="info-menu">
      <li>
        <a href="#">
          <img
            id="w-30"
            src="../assets/buy-comics-digital-comics.png"
            alt="digital-comics"
          />
          <span>DIGITAL COMICS</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/buy-comics-merchandise.png" alt="merchandise" />
          <span>DC MERCHANDISE</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img
            src="../assets/buy-comics-subscriptions.png"
            alt="subscription"
          />
          <span>SUBSCRIPTION</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img
            id="w-30"
            src="../assets/buy-comics-shop-locator.png"
            alt="shop-locators"
          />
          <span>COMIC SHOP LOCATOR</span>
        </a>
      </li>
      <li>
        <a href="#">
          <img src="../assets/buy-dc-power-visa.svg" alt="power-visa" />
          <span>DC POWER VISA</span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "infoComponent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#info-container {
  background-color: #0282f9;
}

.info-menu {
  width: 80%;
  margin: 0 auto;
  list-style-type: none;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-wrap: wrap;
  padding: 40px 0;

  li {
    margin: 10px 20px;

    a {
      text-decoration: none;
      color: white;
      display: flex;
      align-items: center;
      font-size: 14px;

      img {
        width: 40px;
        margin-right: 10px;
      }
    }
  }
}

#w-30 {
  width: 30px;
}
</style>
