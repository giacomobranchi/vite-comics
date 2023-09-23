<script>
import FooterNav from './FooterNav.vue'
import FooterSocial from './FooterSocial.vue';
export default {
  components: {
    FooterNav,
    FooterSocial
  },
  data() {
    return {


    }

  }
}
</script>

<template>
  <FooterNav></FooterNav>
  <div class="background">
    <div class="container">
      <div class="row">
        <div class="col-5">
          <div class="row">
            <div class="col-4">
              <ul class="dc_comics">
                <li>
                  <h5>DC COMICS</h5>
                </li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">Tv</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
              </ul>
              <ul class="shop">
                <li>
                  <h5>SHOP</h5>
                </li>
                <li><a href="#">Shop DC</a></li>
                <li><a href="#">Shop DC Collectibles</a></li>
              </ul>
            </div>
            <div class="col-4">
              <ul class="dc">
                <li>
                  <h5>DC</h5>
                </li>
                <li><a href="#">Terms of Use</a></li>
                <li><a href="#">Privacy Policy (new)</a></li>
                <li><a href="#">Ad Choices</a></li>
                <li><a href="#">Advertising</a></li>
                <li><a href="#">Jobs</a></li>
                <li><a href="#">Subscriptions</a></li>
                <li><a href="#">Talent Workshop</a></li>
                <li><a href="#">CPSC Certificates</a></li>
                <li><a href="#">Ratings</a></li>
                <li><a href="#">Shop Help</a></li>
                <li><a href="#">Contact Us</a></li>
              </ul>
            </div>
            <div class="col-4">
              <ul class="sites">
                <li>
                  <h5>SITES</h5>
                </li>
                <li><a href="#">DC</a></li>
                <li><a href="#">MAD MAGAZINE</a></li>
                <li><a href="#">DC Kids</a></li>
                <li><a href="#">DC Universe</a></li>
                <li><a href="#">DC Power Visa</a></li>
              </ul>
            </div>
          </div>


        </div>
        <div class="col-7">

        </div>
      </div>
    </div>
  </div>
  <FooterSocial></FooterSocial>
</template>

<style lang="scss" scoped>
a {
  text-decoration: none;
  color: grey;
}

ul {
  list-style: none;
  color: white;
}

h5 {
  padding: 1rem 0;
}

.background {
  background-image: url(../assets/img/footer-bg.jpg);
}

.container {



  & .col-7 {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
  }
}
</style>
