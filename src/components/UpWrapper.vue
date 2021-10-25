<template>
  <div class="up-wrapper">

    <img src="../assets/png/Ellipse_39.png" alt="Ellipse" class="ellipse-1">
    <img src="../assets/png/Ellipse_36.png" alt="Ellipse" class="ellipse-2">
    <img src="../assets/png/Ellipse_38.png" alt="Ellipse" class="ellipse-3">
    <img src="../assets/png/Notebook.png" alt="Notebook" class="notebook">
    <S/>
    <Body/>
  </div>
</template>

<script>
import S from '@/components/S.vue'
import Body from "@/components/Body";

export default {
  name: "UpWrapper",
  components: {
    S,
    Body,
  }
}
</script>

<style lang="scss">
.up-wrapper {
  background-color: #001134;
  background-image: url("../assets/png/Vector_6.png"), url("../assets/png/Vector 5.png");
  background-size: 1200px 960px;
  background-position-x: left ;

}

.notebook {
  position: absolute;
  top: 144px;
  right: 164px;
}

.ellipse-1{
  position: absolute;
  width: 387px;
  height: 243px;
  top: 231px;
  right: 213px;
}

.ellipse-2 {
  position: absolute;
  width: 435px;
  height: 368px;
  top: 211px;
  right: 44px;
}

.ellipse-3 {
  position: absolute;
  width: 437px;
  height: 412px;
  top: 100px;
  right: 128px;
}


</style>