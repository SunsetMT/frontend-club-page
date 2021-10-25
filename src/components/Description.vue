<template>
  <div class="description-wrapper">
    <ParaHeader text="Для чего создан клуб"/>
    <ul class="for-points">
      <li class="first">
        <object type="image/svg+xml" :data=this.mySvg></object>
        <StandardText text="начинающие разработчики"/>
      </li>
      <li class="second">
        <object type="image/svg+xml" :data=this.mySvg></object>
        <StandardText text="люди, заинтересованные получить свой первый опыт в разработке реальных кейсов"/>
      </li>
      <li>
        <object type="image/svg+xml" :data=this.mySvg></object>
        <StandardText text="опытные разработчики"/>
      </li>
    </ul>
  </div>
</template>

<script>
import ParaHeader from "@/components/ParaHeader";
import StandardText from "@/components/StandardText";

export default {
  name: "Description",
  components: {
    ParaHeader,
    StandardText
  },
  data() {
    return {
      mySvg: require("../assets/svg/Rectangle-for-li.svg")
    }
  }
}
</script>

<style lang="scss">



.description-wrapper {
  margin-top: 189px;
  color: #ffffff;
  padding-left: 125px;



  ul.for-points {
    margin-top: 21px;
    font-size: 16px;

    li {
      object {
        margin-right: 19px;
      }
      display: flex;
      justify-content: flex-start;
    }

    .first {
      margin-bottom: 16px;
    }
    .second {
      margin-bottom: 17px;
    }

  }
}

@font-face {
  font-family: "Raleway Bold";
  src: url("../assets/fonts/Raleway-Bold.ttf");
}


</style>