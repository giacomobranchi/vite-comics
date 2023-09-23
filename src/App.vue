<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'
export default {
  components: {
    NavBar,
    Footer
  },
  data() {

  }
}
</script>

<template>
  <NavBar></NavBar>
  <div class="bg_black">
    <div class="container">
      <h1 class="m-0 py-4">
        Content Goes Here
      </h1>
    </div>
  </div>
  <Footer></Footer>
</template>

<style>
h1 {
  color: white;

}

.bg_black {
  background-color: black;
}
</style>
