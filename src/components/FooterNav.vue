<script>
import DigitalComics from '../assets/img/buy-comics-digital-comics.png'
import Merchandise from '../assets/img/buy-comics-merchandise.png'
import Subscriptions from '../assets/img/buy-comics-subscriptions.png'
import ShopLocator from '../assets/img/buy-comics-shop-locator.png'
import PowerVisa from '../assets/img/buy-dc-power-visa.svg'
export default {

  data() {
    return {
      name: 'FooterNav',
      DigitalComics,
      Merchandise,
      Subscriptions,
      ShopLocator,
      PowerVisa,
      footerNavLinks: [{
        img: DigitalComics, text: 'DIGITAL COMICS'
      },
      {
        img: Merchandise, text: 'DC MERCHANDISE'
      },
      {
        img: Subscriptions, text: 'SUBSCRIPTIONS'
      },
      {
        img: ShopLocator, text: 'COMIC SHOP LOCATOR'
      },
      {
        img: PowerVisa, text: 'DC POWER VISA'
      },]

    }

  }
}
</script>

<template>
  <div class="band p-5">
    <div class="container">
      <div class="row">
        <div v-for="link in footerNavLinks" class="col">
          <img :src="link.img" alt="">
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
