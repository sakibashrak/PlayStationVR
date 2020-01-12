<template>
  <div class="container">
    <h1>
      The mosy highly anticipated titles
      <br />coming soon to PS VR
    </h1>
    <div class="blackbackground2">
      <div class="blackbackground">
        <div class="poster" v-for="n in 10" :key="n">
          <img :src="`vrgames${n}.png`" />
        </div>
      </div>
    </div>
    <div class="button">
      <app-MainButton class="mainbutton">LEARN MORE</app-MainButton>
    </div>
  </div>
</template>

<script>
import mainbutton from "../components/mainbutton.vue";
export default {
  name: "HomeComingSoon",
  components: {
    appMainButton: mainbutton
  }
};
</script>

<style lang="scss" scoped>
// * {
//   outline: 1px solid yellow;
// }
.container {
  max-width: 100vw;
  overflow: hidden;
  padding-bottom: 80px;
  h1 {
    font-family: "roboto";
    font-size: 2.5rem;
    color: #383838;
    letter-spacing: 0.5px;
    padding-left: 12.5rem;
    padding-top: 8rem;
  }
  .blackbackground2 {
    position: relative;
    margin-top: 70px;
    bottom: -140px;
    height: 500px;
    background-color: #252525;
    z-index: -1;
    .blackbackground {
      position: relative;
      bottom: 140px;
      height: 500px;
      background-color: #252525;
      background-clip: padding-box;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      justify-content: space-around;
      align-content: space-around;
      transform: rotate3d(5, 0, -1, 54deg) scale(1.2, 1.6);
      transform-origin: bottom 0;
      perspective: 1000px;

      .poster {
        transform: translate(0, -60px);
        box-shadow: 0 50px 24px #111;
        img {
          width: 18vw;
          height: 200px;
          object-fit: cover;
        }
      }
    }
  }
  .button {
    display: flex;
    justify-content: flex-end;
    // background-color: #252525;
    padding-right: 10vw;
  }
}

@media screen and (max-width: 960px) {
  .container {
    h1 {
      font-size: 28px;
      padding-left: 9.2rem;
    }
  }
}
</style>
