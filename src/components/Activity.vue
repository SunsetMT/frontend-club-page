<template>
  <div class="activity-wrapper" id="activity">
    <div class="activity-info">
      <div class="activity-info-header">
        <ParaHeader text="Ближайшие мероприятия"/>
      </div>
      <div class="activity-info-text">
        <StandardText text="Не переживай, что ничего глобального пока не происходит — все хакатаны еще будут!"
                      :style="{paddingBottom: 20 + 'px'}"/>
        <StandardText text="А чтобы уж точно ничего не пропустить, подписывайся на нашу группу во “Вконтакте”"/>
      </div>
    </div>
    <object type="image/svg+xml" class="light" :data=this.light></object>
    <EnterButton/>
  </div>
</template>

<script>
import EnterButton from "@/components/EnterButton";
import ParaHeader from "@/components/ParaHeader";
import StandardText from "@/components/StandardText";

export default {
  components: {
    ParaHeader,
    EnterButton,
    StandardText
  },
  name: "Activity",
  data() {
    return {
      light: require("../assets/svg/Light.svg")
    }
  }
}
</script>

<style lang="scss">
.activity-wrapper {
  height: 438px;
  background: #001134;
  color: #ffffff;
  position: relative;


  .activity-info {
    padding-left: 125px;

    .activity-info-header {
      padding-top: 71px;
      margin-bottom: 44px;
    }

    .activity-info-text {
      margin-bottom: 27px;
      width: 488px;
      height: 118px;
      text-align: left;
    }
  }

  .light {
    position: absolute;
    top: 54px;
    right: 212px;
  }
}

</style>