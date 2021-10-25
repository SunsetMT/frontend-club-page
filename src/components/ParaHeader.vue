<template>
  <div class="para-head">
    {{this.text}}
  </div>
</template>

<script>
export default {
  name: "ParaHeader",
  props: {
    text: {
      type: String,
      default: () => {},
    }
  }
}
</script>

<style lang="scss">
.para-head {
  color: #ffffff;
  font-family: "Raleway Bold";
  font-weight: 700;
  margin: 0;
  font-size: 30px;
  display: flex;
  justify-content: flex-start;
}

@font-face {
  font-family: "Raleway Bold";
  src: url("../assets/fonts/Raleway-Bold.ttf");
}

</style>