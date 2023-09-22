<script>
import logo from '../assets/img/dc-logo.png'
export default {
  data() {
    return {
      logo,
      navLinks: ['CHARACTERS', 'COMICS', 'MOVIES', 'TV', 'GAMES', 'COLLECTIBLES', 'VIDEOS', 'FANS', 'NEWS', 'SHOP']
    }

  }
}
</script>

<template>
  <div class="container">
    <nav class="navbar navbar-expand py-4">
      <div class="d-flex justify-content-between w-100">
        <img :src="logo" alt="">
        <div class="nav navbar-nav justify-content-between align-items-center">
          <a v-for="link in navLinks" class="nav-item nav-link border_nav" href="#" aria-current="page">{{ link }}</a>
        </div>

      </div>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
img {
  width: 80px;
}

.border_nav {
  height: 100%;

  &:hover {
    border-bottom: 5px solid blue;
  }
}
</style>
