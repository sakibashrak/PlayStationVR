<template>
  <div class="container">
    <div class="vrimage">
      <img src="../assets/allproducts2.jpg" />
    </div>
    <div class="paragraph">
      <h1>You'll Need These To Get Started</h1>
      <h2>
        PlayStation delivers a new world of unexpected gaming experiences
        through PlayStation VR. Play some of the most highlt anticipated
        coming soon to PS VR
      </h2>
      <div class="mainbutton">
        <app-MainButton>LEARN MORE</app-MainButton>
      </div>
    </div>
  </div>
</template>

<script>
import mainbutton from "../components/mainbutton.vue";
export default {
  name: "HomeIndustryLeadingDesign",
  components: {
    appMainButton: mainbutton
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.container {
  padding-top: 8rem;
  padding-left: 10rem;
  width: 90vw;
  display: flex;
  justify-content: center;
  align-items: center;
  .vrimage {
    height: 30%;
    width: 30%;
    margin-top: 10%;
    object-fit: cover;
    img {
      width: 30vw;
    }
  }
  .paragraph {
    width: 50vw;
    h1 {
      font-family: "roboto";
      font-size: 2.5rem;
      color: #383838;
      letter-spacing: 0.5px;
    }
    h2 {
      color: #7a7a7a;
      font-family: "roboto";
      font-size: 20px;
      font-weight: 100;

      padding-top: 2rem;
    }
    .mainbutton {
      margin-top: 16px;
      letter-spacing: 0px;
      display: flex;
      justify-content: flex-end;
    }
  }
}

@media screen and (max-width: 960px) {
  .container {
    .paragraph {
      h1 {
        font-size: 28px;
      }
    }
  }
}
</style>
