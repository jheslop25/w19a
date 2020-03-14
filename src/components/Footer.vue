<template>
  <div>
    <p>{{ copy }}</p>
  </div>
</template>
<script>
export default {
  name: "Footer",
  props: {
    copy: String
  }
};
</script>
<style scoped>
div {
  width: 100vw;
  height: 10vh;
  background-color: aqua;
}
</style>