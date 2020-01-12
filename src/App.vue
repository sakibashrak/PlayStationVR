<template>
  <div id="app">
    <div id="nav">
      <app-navigationbar></app-navigationbar>
      <!-- router  starts -->
      <!-- <router-link to="/">Home</router-link>| -->
      <!-- <router-link to="/about">About</router-link> -->
      <!-- Router ends -->
    </div>
    <router-view class="routerView" />
    <app-Footer></app-Footer>
  </div>
</template>

<script>
import Navigationbar from "@/components/navigationbar.vue";
import footer from "../src/components/footer.vue";

export default {
  components: {
    appNavigationbar: Navigationbar,
    appFooter: footer
  },
  name: "App",
  data: () => {
    return {};
  }
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Roboto:300,400,500&display=swap");
@import url('https://fonts.googleapis.com/css?family=Audiowide&display=swap');
@import url('https://fonts.googleapis.com/css?family=Expletus+Sans&display=swap');
*,
::before,
::after {
  margin: 0;
  box-sizing: border-box;
}
.html {
  font-size: 16px;
  font-family: "Roboto", sans-serif;
}

#app {
  min-height: 100vh;
  position: relative;
}
.routerView {
  padding-bottom: 12vh;
}
</style>
