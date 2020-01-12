<template>
  <div class="container">
    <div class="tagline">
      <h2>
        Discover a new would of unexpected
        <br />gaming and entertainment experiences
      </h2>
      <div class="titleline">
        <h1>
          PlayStation
          <!-- <span>&copy;</span> -->
          VR
        </h1>
      </div>

      <app-MainButton class="mainbutton">LEARN MORE</app-MainButton>
    </div>
  </div>
</template>

<script>
import mainbutton from "../components/mainbutton.vue";
export default {
  name: "HomeTopPicture",
  components: {
    appMainButton: mainbutton
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.container {
  height: calc(100vh - 80px);
  min-height: 400px;
  overflow: hidden;
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: repeat(4, 1fr);
  // justify-content: space-around;
  // align-items: center;
  .tagline {
    grid-area: 2 / 2;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 2rem;
    border-radius: 0.5rem;
    background: #ffffffcc;
    & > * {
      margin: 12px 0;
    }
    h2 {
      font-family: "roboto";
      font-weight: 50;
      color: rgb(153, 153, 153);
      font-size: 24px;
    }
    span {
      font-size: 1rem;
      white-space: nowrap;
      // color: red
    }
  }
  .titleline {
    h1 {
      // font-family: 'Audiowide', cursive;
      font-family: "Expletus Sans", cursive;
      font-size: 4rem;
      color: 46, 46, 46;
    }
  }
  // .mainbutton {
  //   font-family: "roboto";
  //   letter-spacing: 2px;
  //   color: white;
  //   background-color: #2787db;
  //   font-size: 18px;
  //   font-weight: 500;
  //   padding: 14px;
  //   border-radius: 40px;
  // }
}
@media screen and (max-width: 960px) {
  .container {
    height: calc(100vh - 450px);
    grid-template-columns: 1fr 1fr;
    grid-template-rows: repeat(10, 1fr);
    .tagline {
      grid-area: 2 / 2;
      padding: 0rem;
      h2 {
        font-size: 20px;
      }
      .titleline {
        h1 {
          font-size: 36px;
        }
      }
    }
  }
}
</style>
