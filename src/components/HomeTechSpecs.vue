<template>
  <div class="maincontainer">
    <div class="container">
      <h1>Tech Specs</h1>
      <hr class="bordertop" />
      <div class="footerinfo">
        <div class="footerinfo1">
          <h2>External Dimensions</h2>
          <p>
            VR headset: Approx. 187x185x277 mm (width x height x length,
            excludes largest projection, headband at the shortest)
            Processor unit: Approx. 143x36x143 mm (width x height x length
            excludes largesr projection)
          </p>
          <h2>Mass</h2>
          <p>
            VR headset: Approx. 620g (excluding cable)
            Processor Unit: Approx. 365g
          </p>
          <h2>Display</h2>
          <p>
            5.7 Inches OLED 1920 x RGB x 1080 (960 x RGB x 1080 / eye)
            120Hzs, 90Hz REfresh rate
          </p>
        </div>
        <div class="footerinfo2">
          <h2>Sensors</h2>
          <p>
            Six-axis motion sensing system (three-axis gyroscope,
            three-axis accelerometer
          </p>
          <h2>Connection Interface</h2>
          <p>
            Vr headset: HDMI, AUX, Stereo Headphone Jack
            Processor unit: HDMI TV, HDMI PS4, USB, HDMI, AUX
          </p>
          <h2>Processor Unit Function</h2>
          <p>
            3D audio processor, Social Screen (mirroring mode,
            seperate mode), Cinematic mode
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  background-color: #252525;
  padding: 10px 10vw 80px;
  h1 {
    color: #fcfcfc;
    font-family: "roboto";
    font-weight: 800;
    font-size: 36px;
    padding-left: 0px;
    padding-bottom: 36px;
  }

  .footerinfo {
    .footerinfo1 {
      width: 50vw;
    }
    .footerinfo2 {
      width: 50vw;
      padding-left: 8vw;
    }
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    h2 {
      color: #fcfcfcf6;
      font-family: "roboto";
      font-weight: 400;
      font-size: 20px;
      padding-top: 46px;
    }
    p {
      color: #a1a1a1;
      font-family: "roboto";
      font-size: 20px;
      line-height: 1.7;
    }
  }
}
.maincontainer {
}
@media screen and (max-width: 960px) {
  .container {
    padding: 10px 2vw 80px;
    h1 {
      font-size: 28px;
    }
  }
}
</style>
