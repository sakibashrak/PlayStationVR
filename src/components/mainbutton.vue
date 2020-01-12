<template>
  <button class="mainbutton">
    <slot>Button</slot>
  </button>
</template>

<style lang="scss" scoped>
.mainbutton {
  font-family: "roboto";
  letter-spacing: 1px;
  color: white;
  background-color: #2787db;
  font-size: 18px;
  font-weight: 500;
  padding: 14px 28px 14px 28px;
  border-radius: 40px;
  border: 0;
  outline:none;
 cursor:pointer;
}
</style>
