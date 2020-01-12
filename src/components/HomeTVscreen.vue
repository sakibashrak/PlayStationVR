<template>
  <div class="container">
    <img class="TVscreen" src="../assets/mainTVscreen.jpg" />
  </div>
</template>

<script>
export default {};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.container {
  display: flex;
  justify-content: center;
  padding-top: 72px;
  .TVscreen {
    box-shadow: 0 0 4rem #333;
    width: 50vw;
  }
}

@media screen and (max-width: 960px) {
  .container {
    .TVscreen {
      // width: 50vw;
    }
  }
}
</style>
