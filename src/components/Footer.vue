<template>
  <footer>
    <div id="container-nav">
      <div class="footer-left-nav">
        <h2>DC COMICS</h2>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
        <h2 class="m-top">SHOP</h2>
        <ul>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>

      <div class="footer-center-nav">
        <h2>DC</h2>
        <ul>
          <li>
            <a href="#">Terms Of Use</a>
          </li>
          <li>
            <a href="#">Privacy Policy</a>
          </li>
          <li>
            <a href="#">Ad Choices</a>
          </li>
          <li>
            <a href="#">Advertising</a>
          </li>
          <li>
            <a href="#">Jobs</a>
          </li>
          <li>
            <a href="#">Subscriptions</a>
          </li>
          <li>
            <a href="#">Talent Workshops</a>
          </li>
          <li>
            <a href="#">CPSC Certificates</a>
          </li>
          <li>
            <a href="#">Ratings</a>
          </li>
          <li>
            <a href="#">Shop Help</a>
          </li>
          <li>
            <a href="#">Contact Us</a>
          </li>
        </ul>
      </div>

      <div class="footer-right-nav">
        <h2>SITES</h2>
        <ul>
          <li>
            <a href="#">DC</a>
          </li>
          <li>
            <a href="#">MAD Magazine</a>
          </li>
          <li>
            <a href="#">DC Kids</a>
          </li>
          <li>
            <a href="#">DC Universe</a>
          </li>
          <li>
            <a href="#">DC Power Visa</a>
          </li>
        </ul>
      </div>

      <div class="img"></div>
    </div>

    <div class="w-100">
      <div id="sign-follow">
        <div class="sign-now">
          <button type="button"><strong>SIGN-UP NOW!</strong></button>
        </div>
        <div class="follow-us">
          <h2>FOLLOW US</h2>
          <ul class="icon-list">
            <li>
              <a href="#">
                <img src="../assets/footer-facebook.png" alt="Facebook" />
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-twitter.png" alt="Twitter" />
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-youtube.png" alt="Youtube" />
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-pinterest.png" alt="Pinterest" />
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-periscope.png" alt="Periscope" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "footerComponent",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}

#container-nav {
  width: 80%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;

  .footer-left-nav,
  .footer-center-nav,
  .footer-right-nav {
    padding: 40px 0;
  }

  .img {
    flex-grow: 1;
    background-image: url("../assets/dc-logo-bg.png");
    background-repeat: no-repeat;
    background-position: center right;
  }
}

h2 {
  color: white;
  font-size: 14px;
  margin-bottom: 5px;
}

ul {
  list-style-type: none;
  margin-right: 20px;

  a {
    color: #999;
    text-decoration: none;
    font-size: 10px;
  }
}

#sign-follow {
  width: 80%;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 30px 0;

  button {
    padding: 10px;
    margin-bottom: 5px;
    background: none;
    color: white;
    border: none;
    outline: 2px solid #008dff;
  }

  .follow-us {
    display: flex;
    align-items: center;
    flex-wrap: wrap;

    h2 {
      margin-right: 15px;
      color: #008dff;
    }

    .icon-list {
      display: flex;
      flex-wrap: wrap;

      li {
        margin: auto 8px;
      }
    }
  }
}

.m-top {
  margin-top: 10px;
}

.w-100 {
  width: 100%;
  background-color: #303030;
}
</style>
