<template>
  <div class="container">
    <div class="blackstrip">
      <h2>SONY</h2>
    </div>
    <div class="TopNavigation">
      <router-link to="/" tag="img" src="pslogo2.png"></router-link>
      <div class="flexGrow"></div>
      <div class="navBar">
        <router-link
          v-for="item in items"
          :key="item.text"
          :to="`${item.link}`"
          exact-active-class="active"
        >{{ item.text }}</router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      items: [
        { text: "PS4", link: "/ps4" },
        { text: "PSVR", link: "/" },
        { text: "GAMES", link: "/games" },
        { text: "NEWS", link: "/news" },
        { text: "PSN", link: "/psn" },
        { text: "STORE", link: "/store" }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
.container {
  .blackstrip {
    background-color: #222;
    height: 5vh;
    display: flex;
    align-items: center;
    justify-content: flex-end;
    h2 {
      font-family: "Times New Roman", Times, serif;
      color: white;
      padding-right: 20px;
    }
  }
  .TopNavigation {
    img {
      height: 3.5vh;
      margin: 2rem 2rem;
      cursor: pointer;
    }
    align-items: baseline;
    overflow: hidden;
    display: flex;
    flex-direction: row;
    height: 100px;
    h1 {
      padding: 0 1rem;
    }
    .flexGrow {
      flex-grow: 1;
    }
    a {
      font-family: "roboto";
      color: #222;
      text-align: center;
      padding: 0.5rem 0.5rem;
      margin: 0.25rem 1rem;
      text-decoration: none;
      font-size: 17px;
      position: relative;
      &:active {
        color: #222;
      }
      &::after {
        content: "";
        width: 100%;
        position: absolute;
        bottom: 0;
        left: 0;
        border-radius: 4px;
        height: 0px;
        background: #2787db;
        transition: all 0.2s ease-in-out;
      }
      &:hover,
      &.active {
        font-weight: 500;
      }
      &.active::after {
        height: 4px;
      }
    }
  }
}
</style>
