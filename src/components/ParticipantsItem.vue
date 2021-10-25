<template>
  <div class="par-item">
    <div class="par-img">
      <img :src="require(`../assets/png/${this.parItem.png}`)" alt="">
    </div>
    <div class="par-name">
      {{ this.parItem.name }}
    </div>
  </div>
</template>

<script>
export default {
  name: "ParticipantsItem",
  props: {
    parItem: {
      type: Object,
      default: () => {
      }
    }
  }
}
</script>

<style lang="scss">

.par-item {
  padding-right: 75px;
  .par-img {

  }
  .par-name {
    padding-top: 19px;
    font-family: "Roboto Medium";
    text-transform: uppercase;
    font-weight: 500;
    color: #ffffff;
  }
}

@font-face {
  font-family: "Roboto Medium";
  src: url("../assets/fonts/Roboto-Medium.ttf");
}

</style>