<template>
  <button :class="color">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "ButtomApp",
  props: {
    color: {
      type: String,
      default: "primary",
    },
  },
};
</script>

<style scoped>
button {
  padding: 10px 15px;

  border: none;
  outline: none;
  border-radius: 10px;
  color: white;
  font-weight: bold;
}
.segundari{
    background-color: rgb(108, 00, 117)
}
.primary {
  background-color: rgb(108, 200, 117);
}
</style>
