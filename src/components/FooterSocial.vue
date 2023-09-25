<script>

export default {
  data() {
    return {
      name: 'FooterSocial',
      footerSocialLinks: [{
        name: 'facebook', icon: '../assets/img/footer-facebook.png'
      }, {
        name: 'twitter', icon: '../assets/img/footer-twitter.png'
      },
      {
        name: 'youTube', icon: '../assets/img/footer-youtube.png'
      },
      {
        name: 'pinterest', icon: '../assets/img/footer-pinterest.png'
      },
      {
        name: 'periscope', icon: '../assets/img/footer-periscope.png'
      },
      ]
    }

  },
  methods: {
    getImageUrl(name) {
      return new URL(`${name}`, import.meta.url).href
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
            <img class="px-1 py-5" v-for="link in footerSocialLinks" :src="getImageUrl(link.icon)">
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
