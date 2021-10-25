<template>
  <div class="mentors-slider-item">
    <div class="mentor-image" :style="styleObject">
      <img :src="require(`../assets/png/${this.mentorsItem.png}`)" alt="" class="mentor-png">

    </div>
    <div class="mentor-name"
         v-if="mentorsItem.png === `Ruslan.png`"
         :style="{'font-family': 'Roboto Medium' , 'font-weight': '500'}">{{this.mentorsItem.name}}
    </div>
    <div class="mentor-name"
         v-else
         :style="{'font-family': 'Roboto Bold', 'font-weight': '700'}">{{this.mentorsItem.name}}
    </div>

  </div>

</template>

<script>
export default {
  name: "MentorsSliderItem",
  props: {
    mentorsItem: {
      type: Object,
      default: () => {}
    }
  },
  computed: {
    styleObject: function (){
      return{
        //background: 'no-repeat center/100% ' + 'url(' + require(`../assets/png/${this.mentorsItem.png}`) + ')'
      }
    }
  }
}
</script>

<style lang="scss">

.mentors-slider-item{
  margin-right: 43px;
  width: 260px;
  height: 295px;

  position: relative;
  z-index: 3;

  .mentor-image{
    width: 260px;
    height: 260px;
  }

  .mentor-name{
    color: #ffffff;
    font-size: 16px;
    text-transform: uppercase;
    margin-top: 13px;
  }
}

.mentor-png{

}

@font-face {
  font-family: "Roboto Bold";
  src: url("../assets/fonts/Roboto-Bold.ttf");
}

@font-face {
  font-family: "Roboto Medium";
  src: url("../assets/fonts/Roboto-Medium.ttf");
}



</style>