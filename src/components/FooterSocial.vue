<script>
import facebook from '../assets/img/footer-facebook.png'
import twitter from '../assets/img/footer-twitter.png'
import youTube from '../assets/img/footer-youtube.png'
import pinterest from '../assets/img/footer-pinterest.png'
import periscope from '../assets/img/footer-periscope.png'
export default {
  data() {
    return {
      facebook,
      twitter,
      youTube,
      pinterest,
      periscope,
      footerSocialLinks: [facebook, twitter, youTube, pinterest, periscope]
    }

  }
}
</script>

<template>
  <div class="footer_social">
    <div class="container">
      <div class="row justify-content-between align-items-center">
        <div class="col-2">
          <a class="signup">SIGN UP NOW!</a>
        </div>
        <div class="col-4">
          <div>
            <h5 class="d-inline px-4">FOLLOW US</h5>
            <img class="px-1 py-5" v-for="link in footerSocialLinks" :src="link">
          </div>
        </div>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
h5 {
  color: #0282f9;
}

.footer_social {
  background-color: #303030;
}

.signup {
  color: white;
  text-decoration: none;
  padding: 1rem;
  border: 2px solid #0282f9;
}
</style>
