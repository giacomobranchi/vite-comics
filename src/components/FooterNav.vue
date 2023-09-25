<script>

export default {

  data() {
    return {
      name: 'FooterNav',
      footerNavLinks: [{
        img: '../assets/img/buy-comics-digital-comics.png', text: 'DIGITAL COMICS'
      },
      {
        img: '../assets/img/buy-comics-merchandise.png', text: 'DC MERCHANDISE'
      },
      {
        img: '../assets/img/buy-comics-subscriptions.png', text: 'SUBSCRIPTIONS'
      },
      {
        img: '../assets/img/buy-comics-shop-locator.png', text: 'COMIC SHOP LOCATOR'
      },
      {
        img: '../assets/img/buy-dc-power-visa.svg', text: 'DC POWER VISA'
      },]

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
  <div class="band p-5">
    <div class="container">
      <div class="row align-items-center">
        <div v-for="link in footerNavLinks" class="col d-flex align-items-center">
          <div class="img_container" :style="{ 'background-image': 'url(' + getImageUrl(link.img) + ')' }">
            <!-- <img :src="getImageUrl(link.img)" alt=""> -->
          </div>
          <div class="p-2 small">{{ link.text }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.band {
  background-color: #0282f9;
  color: white;

  & .img_container {
    display: inline-block;
    height: 60px;
    aspect-ratio: 1;
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain;
  }


}
</style>
