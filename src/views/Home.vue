<template>
  <div class="home">
    <app-HomeTopPicture></app-HomeTopPicture>
    <app-HomeTVscreen></app-HomeTVscreen>
    <app-HomeIndustryLeadingDesign></app-HomeIndustryLeadingDesign>
    <app-Homecarousel></app-Homecarousel>
    <app-HomeGetStarted></app-HomeGetStarted>
    <app-HomeComingSoon></app-HomeComingSoon>
    <app-HomeTechSpecs></app-HomeTechSpecs>
    <!-- <h1>This is home.vue</h1> -->
  </div>
</template>

<script>
// @ is an alias to /src

import HomeTopPicture from "../components/HomeTopPicture.vue";
import HomeTVscreen from "../components/HomeTVscreen.vue";
import HomeIndustryLeadingDesign from "../components/HomeIndustryLeadingDesign.vue";
import Homecarousel from "../components/Homecarousel.vue";
import HomeGetStarted from "../components/HomeGetStarted.vue";
import HomeComingSoon from "../components/HomeComingSoon.vue";
import HomeTechSpecs from "../components/HomeTechSpecs.vue";

export default {
  name: "home",
  components: {
    appHomeTopPicture: HomeTopPicture,
    appHomeTVscreen: HomeTVscreen,
    appHomeIndustryLeadingDesign: HomeIndustryLeadingDesign,
    appHomecarousel: Homecarousel,
    appHomeGetStarted: HomeGetStarted,
    appHomeComingSoon: HomeComingSoon,
    appHomeTechSpecs: HomeTechSpecs
  }
};
</script>

<style lang="scss" scoped>
.home {
  background: url("../assets/main4.png");
  background-repeat: no-repeat;
  background-size: 100vw;
}
</style>
