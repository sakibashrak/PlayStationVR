<template>
  <div class="maincontainer">
    <div class="bluestrip">
      <h2>2016 Sony Interactive Entertainment LLC</h2>
      <img src="../assets/pslogo4.png" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.maincontainer {
  position: absolute;
  width: 100%;
  bottom: 0;
  .bluestrip {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    align-items: center;
    height: 12vh;
    background: rgb(8, 63, 146);
    background: linear-gradient(
      124deg,
      rgba(8, 63, 146, 1) 0%,
      rgba(11, 86, 170, 1) 35%,
      rgba(20, 112, 197, 1) 100%
    );

    padding: 0px;
    h2 {
      color: white;
      font-family: "roboto";
      font-size: 20px;
      font-weight: 200;
    }
    img {
      height: 3.5vh;
      color: white;
    }
  }
}
</style>
