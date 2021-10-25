<template>
  <div class="standard-text">
    {{ this.text }}
  </div>
</template>

<script>
export default {
  name: "StandardText",
  props: {
    text: {
      type: String,
      default: () => {
      }
    }
  }
}
</script>

<style lang="scss">

.standard-text {
  color: #ffffff;
  font-family: "Roboto Regular";
  font-size: 16px;
  line-height: 140%;
}

@font-face {
  font-family: "Roboto Regular";
  src: url("../assets/fonts/Roboto-Regular.ttf")
}
</style>