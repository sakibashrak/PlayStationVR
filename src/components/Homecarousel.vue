<template>
  <div class="glide">
    <div data-glide-el="track" class="glide__track">
      <ul class="glide__slides">
        <div class="glide__slide" v-for="n in 9" :key="n">
          <img :src="`s${n}.jpeg`" />
        </div>
      </ul>
    </div>
    <div class="glide__bullets" data-glide-el="controls[nav]">
      <button class="glide__bullet" data-glide-dir="=0"></button>
      <button class="glide__bullet" data-glide-dir="=1"></button>
      <button class="glide__bullet" data-glide-dir="=2"></button>
      <button class="glide__bullet" data-glide-dir="=3"></button>
      <button class="glide__bullet" data-glide-dir="=4"></button>
      <button class="glide__bullet" data-glide-dir="=5"></button>
      <button class="glide__bullet" data-glide-dir="=6"></button>
    </div>
  </div>
</template>

<script>
import Glide, {
  Controls,
  Breakpoints
} from "@glidejs/glide/dist/glide.modular.esm";

export default {
  data: () => {
    return {
      glide: null
    };
  },
  mounted() {
    this.glide = new Glide(".glide", {
      type: "slider",
      startAt: 0,
      perView: 3,
      gap: 20,
      peek: 200
    });
    // console.log(glide);
    this.glide.mount({ Controls, Breakpoints });
  }
};
</script>
<style lang="scss" scoped>
// Required Core Stylesheet
@import "node_modules/@glidejs/glide/src/assets/sass/glide.core";
// Optional Theme Stylesheet
@import "node_modules/@glidejs/glide/src/assets/sass/glide.theme";

.glide__slide {
  height: 300px;
  width: 100px;
  margin-top: 80px;
  margin-bottom: 80px;

  // background: #3273ef;
  border: 0.15rem solid #2787db;
  box-shadow: 0 0 0.5rem #333;
  img {
    height: 100%;
    width: 100%;
    object-fit: cover;
  }
}
.glide__bullet {
  display: flex;
  justify-content: center;
  align-items: flex-end;

  box-shadow: 0 0 0.1rem #333;
  background-color: #e2e2e2;
  width: 0.75rem;
  height: 0.75rem;
  margin-left: 0.3rem;
  &:hover {
    background-color: darken(#e2e2e2, 10%);
    border: none;
  }
  &:focus {
    border: none;
  }
}
.glide__bullet--active {
  background-color: #007cdb !important;
}

@media screen and (max-width: 960px) {
  .glide__slide {
    height: 200px;
    width: 100px;
    margin-top: 80px;
    margin-bottom: 80px;

    // background: #3273ef;
    border: 0.15rem solid #2787db;
    box-shadow: 0 0 0.5rem #333;
    img {
      height: 100%;
      width: 100%;
      object-fit: cover;
    }
  }
}
</style>
