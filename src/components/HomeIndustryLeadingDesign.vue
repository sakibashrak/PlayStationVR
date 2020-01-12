<template>
  <div class="container">
    <div class="paragraph">
      <h1>Industry Leading Design</h1>
      <h2>
        The PlayStation VR headset was engineered to be balanced,
        confortable and completely adjustable. It's designed to feel like
        it's not there keeping you free from distraction ans you explore
        new gaming worlds
      </h2>
      <div class="mainbutton">
        <app-MainButton>LEARN MORE</app-MainButton>
      </div>
    </div>
    <div class="vrimage">
      <img src="../assets/vrheadset.jpg" />
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
  padding-left: 5rem;
  display: flex;
  justify-content: center;
  align-items: center;

  .paragraph {
    width: 50vw;
    // border-radius: 32px;
    // padding: 32px;
    //  box-shadow: -20px 20px 30px 1px rgba(233, 230, 224, 0.623);
    // //  up to last line to put shadows
    // border-left: 5px ridge rgba(233, 230, 224, 0.055);
    // border-bottom: 5px ridge rgba(233, 230, 224, 0.055);

    // border-bottom: #7a7a7a solid 1px;

    // box-shadow: 0 0 0.5rem #333;

    // padding-bottom: 32px;
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
    }
  }
  .vrimage {
    height: 30%;
    width: 30%;

    object-fit: cover;
    img {
      width: 30vw;
    }
  }
}

@media screen and (max-width: 960px) {
  .container {
    padding-top: 8rem;
    padding-left: 5rem;

    .paragraph {
      h1 {
        font-size: 28px;
        letter-spacing: 0.5px;
      }
      h2 {
        font-size: 20px;
        font-weight: 100;
        padding-top: 2rem;
      }
      .mainbutton {
        margin-top: 16px;
        letter-spacing: 0px;
      }
    }
  }
}
</style>
