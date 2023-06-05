<script>
export default {
  name: "AppFooter",

  data() {
    return {
      jumbrotronLinks: [
        {
          text: "DIGITAL COMICS",
          img: "../src/assets/img/buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          img: "../src/assets/img/buy-comics-merchandise.png",
        },
        {
          text: "SUBSCRIPTION",
          img: "../src/assets/img/buy-comics-subscriptions.png",
        },
        {
          text: "COMIC SHOP LOCATOR",
          img: "../src/assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          img: "../src/assets/img/buy-dc-power-visa.svg",
        }

      ],
    }
  }
}
</script>


<template>
  <div class="footer">
    <div class="container">
      <ul>
        <li v-for="link in jumbrotronLinks">
          <img :src="link.img">
          {{ link.text }}
        </li>
      </ul>
    </div>
  </div>
  <div class="background-footer">
    <div class="container">
      <div class="site-map-1">
        <div>
          <span>DIGITAL COMICS</span>
          <ul>
            <li>
              Character
            </li>
            <li>
              Comics
            </li>
            <li>
              Movie
            </li>
            <li>
              TV
            </li>
            <li>
              Games
            </li>
            <li>
              Videos
            </li>
            <li>
              News
            </li>
          </ul>
          <span>SHOP</span>
          <ul>
            <li>
              Shop DC
            </li>
            <li>
              Shop DC Collectible
            </li>
          </ul>
        </div>
      </div>
      <div class="site-map-2">
        <span>DC</span>
        <ul>
          <li>
            Term Of Use
          </li>
          <li>
            Privacy policy
          </li>
          <li>
            Ad Choices
          </li>
          <li>
            Advertising
          </li>
          <li>
            Jobs
          </li>
          <li>
            Subscriptions
          </li>
          <li>
            Talent Workshop
          </li>
          <li>
            CPSC Certificates
          </li>
          <li>
            Rating
          </li>
          <li>
            Shop Help
          </li>
          <li>
            Contact Us
          </li>
        </ul>
      </div>
      <div class="site-map-3">
        <span>SITES</span>
        <ul>
          <li>
            DC
          </li>
          <li>
            MAD Magazine
          </li>
          <li>
            DC Kids
          </li>
          <li>
            DC Universe
          </li>
          <li>
            DC Power Visa
          </li>
        </ul>
      </div>
    </div>
  </div>
  <div class="reference-footer">
    <div class="container">
      <button>
        SIGN UP NOW!
      </button>
      <div class="social-network">
        <span>
          FOLLOW US
        </span>
        <i class="fa-brands fa-facebook"></i>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-youtube"></i>
        <i class="fa-brands fa-pinterest"></i>
        <i class="fa-solid fa-location-dot"></i>

      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../styles/partiarls/mixins.scss' as *;
@use '../styles/partiarls/colors.scss' as *;

.footer {
  height: 100px;
  background-color: $dcBlue;

  .container {

    ul {
      @include my-dislay-flex;
      height: 100px;
      font-size: 10px;

      li {
        color: white;

        img {
          width: 35px;
          height: 40px;
          vertical-align: middle;
          margin-right: 10px;
        }
      }
    }
  }
}

.background-footer {
  background-image: url(../assets/img/footer-bg.jpg);


  .container {
    padding: 30px 0px;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;

    .site-map-1,
    .site-map-2,
    .site-map-3 {
      display: inline-block;
      padding-right: 50px;
      vertical-align: top;


      span {
        color: white;
        font-weight: bold;
      }

      ul {
        font-size: 10px;
        color: $footerGray;

      }
    }
  }
}

.reference-footer {
  background-color: #303030;

  .container {

    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;

    button {
      padding: 5px 10px;
      color: white;
      border: 2px solid $dcBlue;
      background-color: #303030;
    }

    .social-network {
      span {
        color: $dcBlue;
        font-weight: bold;
      }

      i {
        padding: 0px 5px;
        font-size: 22px;
        color: $footerGray;
        vertical-align: middle;
      }
    }
  }
}
</style>
