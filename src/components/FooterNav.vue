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
      <div class="row">
        <div v-for="link in footerNavLinks" class="col">
          <img :src="getImageUrl(link.img)" alt="">
          <span class="p-2">{{ link.text }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.band {
  background-color: #0282f9;
  color: white;

  & img {
    height: 60px;
  }
}
</style>
