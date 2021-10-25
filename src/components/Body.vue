<template>
  <div class="body-wrapper" :style="{backgroundImage: back1}">
    <div class="club-and-img">
      <h1 class="club-title">Клуб фронтенд разработки FTML</h1>

    </div>
    <div class="club-short-description">
      <StandardText
          text="Хочешь заниматься фронтендом или уже что-то умеешь? Вступай в наш клуб и найти единомышленников"/>
    </div>

    <EnterButton/>
    <Description/>
    <MotivationCard/>
    <Activity/>
    <Mentors/>
    <Participants/>
    <Footer/>
  </div>
</template>

<script>
import Mentors from "@/components/Mentors";
import StandardText from "@/components/StandardText";
import EnterButton from "@/components/EnterButton";
import Description from "@/components/Description";
import MotivationCard from "@/components/MotivationCard";
import Activity from "@/components/Activity";
import Participants from "@/components/Participants";
import Footer from "@/components/Footer";


export default {
  components: {
    StandardText,
    EnterButton,
    Description,
    MotivationCard,
    Activity,
    Mentors,
    Participants,
    Footer
  },
  name: "Body",
  data() {
    return {
      back1: "../assets/png/Notebook.png"
    }
  }
}
</script>

<style lang="scss">
.body-wrapper {

  padding-top: 83px;
  height: 806px;

  h1 {
    margin: 0;
    text-align: left;
  }

  .club-and-img {
    display: flex;


  }

  .club-title {
    color: #ffffff;
    font-family: "Raleway Bold";
    font-size: 48px;
    line-height: 110%;
    width: 437px;
    height: 98px;
    margin-bottom: 25px;
    padding-left: 125px;

  }

  .club-short-description {
    text-align: left;
    width: 444px;
    height: 44px;
    padding-left: 125px;
    padding-bottom: 25px;
  }



}


@font-face {
  font-family: "Raleway Bold";
  src: url("../assets/fonts/Raleway-Bold.ttf");
}

@font-face {
  font-family: "Raleway Regular";
  src: url("../assets/fonts/Raleway-Regular.ttf");
}

</style>