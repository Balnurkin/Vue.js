<script>
export default {
  name: "MyButtonGr",
};
</script>

<template>
  <button class="my-button">
    <slot></slot>
  </button>
</template>

<style scoped>
.my-button {
  width: 200px;
  height: 49px;
  border: 1px solid #3c5f41;
  border-radius: 24px;
  background-color: #55885d;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  color: white;
}
</style>
