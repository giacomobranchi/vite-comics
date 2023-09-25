<script>
import NavBar from './components/NavBar.vue'
import AppFooter from './components/AppFooter.vue'
import AppMain from './components/AppMain.vue'
export default {
  components: {
    NavBar,
    AppFooter,
    AppMain
  },
  data() {

  }
}
</script>

<template>
  <NavBar></NavBar>
  <!-- <div class="bg_black">
    <div class="container">
      <h1 class="m-0 py-4">
        Content Goes Here
      </h1>
    </div>
  </div> -->
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style>
h1 {
  color: white;

}

.bg_black {
  background-color: black;
}
</style>
