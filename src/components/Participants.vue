<template>
  <div class="participants-wrapper" id="participants">
    <div class="par-box">
      <div class="par-header">
        <ParaHeader text="Участники"/>
      </div>
      <div class="par-list">
        <ParticipantsItem
            v-for="item in items"
            :key="item.id"
            :par-item="item"
        />
      </div>
    </div>
  </div>
</template>

<script>
import ParaHeader from "@/components/ParaHeader";
import ParticipantsItem from "@/components/ParticipantsItem";

export default {
  name: "Participants",
  components: {
    ParaHeader,
    ParticipantsItem
  },
  data() {
    return {
      items: [
        {name: "Сулейманов Руслан ", png: "Ellipse_2.png", id: 1},
        {name: "Сулейманов Руслан ", png: "Ellipse_2.png", id: 2},
        {name: "Сулейманов Руслан ", png: "Ellipse_2.png", id: 3},
        {name: "Сулейманов Руслан ", png: "Ellipse_2.png", id: 4},
        {name: "Сулейманов Руслан ", png: "Ellipse_2.png", id: 5},
      ]
    }
  }
}
</script>

<style lang="scss">

.participants-wrapper {
  width: 1200px;
  height: 437px;
  overflow: hidden;
  background-color: #001134;

  .par-box {
    padding-left: 125px;
  }

  .par-header {
    padding-top: 53px;
  }

  .par-list {
    display: flex;
    margin-top: 42px;
  }

}

</style>