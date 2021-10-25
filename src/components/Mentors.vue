<template>
  <div class="mentors-wrapper" id="mentors">
    <img src="../assets/png/Vector_9.png" alt="Vector" class="vector-9">
    <img src="../assets/png/Vector_8.png" alt="Vector" class="vector-8">



    <div class="mentors-box">
      <div class="mentors-head">
        <ParaHeader text="Руководители"/>
      </div>

      <div class="mentors-slider" :style="this.styleObject">
        <MentorsSliderItem
            v-for="item in items"
            :key="item.id"
            :mentors-item="item"
        />
      </div>

      <div class="slider-nav">
        <div class="a2">
          <button v-on:click="this.dec">
            <img src="../assets/png/Arrow_2.png" alt="arrow-2" class="arrow-2">
          </button>
        </div>
        <div class="nav-1"><img src="../assets/png/Rectangle_54.png" alt="nav-scroll" class="nav-scroll"></div>
        <div class="a1">
          <button v-on:click="this.inc">
            <img src="../assets/png/Arrow_1.png" alt="arrow-1" class="arrow-1">
          </button>
        </div>
      </div>

      <img src="../assets/png/Rectangle_55.png" alt="" class="bar" :style="barStyle">

    </div>
  </div>
</template>

<script>
import ParaHeader from "@/components/ParaHeader";
import MentorsSliderItem from "@/components/MentorsSliderItem";

export default {
  name: "Mentors",
  components: {
    ParaHeader,
    MentorsSliderItem
  },
  data() {
    return {
      items: [
        {name: "Сулейманов Руслан", png: "Ruslan.png", id: 1},
        {name: "Береснев Андрей", png: "Andrew.png", id: 2},
        {name: "Прохоров Николай", png: "Nikolay.png", id: 3},
        {name: "Прохоров Николай", png: "Nikolay.png", id: 4},
      ],
      cnt:0,
    }
  },
  methods: {
    inc() {
      if(this.cnt < 1) this.cnt++;
    },
    dec() {
      if(this.cnt > 0) this.cnt--;
    }
  },
  computed: {
    styleObject(){
      return{
        'margin-left': -303 * this.cnt + 'px'
      }
    },
    barStyle() {
      return {
        'left': 197 + 650 * this.cnt + 'px'

      }
    }
  }
}
</script>

<style lang="scss">

.mentors-wrapper {
  display: block;
  width: 1200px;
  height: 594px;
  background-color: #121F4D;
  position: relative;
  overflow: hidden;
}

.vector-9 {
  z-index: 1;
  position: absolute;
  width: 1078px;
  height: 594px;
  top: 0;
  right: 18px;
}

.vector-8 {
  z-index: 2;
  position: absolute;
  width: 1056px;
  height: 594px;
  top: 0;
  right: 144px;
}


.mentors-head {
  padding-top: 53px;
}

.mentors-box {
  padding-left: 125px;

  .mentors-slider {
    overflow: hidden;
    max-width: 1200px;
    display: flex;
    margin-top: 73px;
    transition: all ease 0.5s;
  }
}

.bar {
  position: absolute;
  top: 514px;
  left: 197px;
  z-index: 3;
  transition: all ease 0.5s;
}


.slider-nav {
  position: relative;
  z-index: 3;
  display: flex;
  padding-top: 40px;
  width: 950px;
  justify-content: space-between;
  align-items: center;

  button{
    background: inherit;
    border: inherit;
  }

  .arrow-2 {

  }

  .nav-scroll {
    padding-bottom: 6px;
  }
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