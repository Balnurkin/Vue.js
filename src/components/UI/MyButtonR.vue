<script>
export default {
  name: "MyButtonR",
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
  border: 1px solid #844154;
  border-radius: 24px;
  background-color: #bc5d78;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  color: white;
}
</style>
