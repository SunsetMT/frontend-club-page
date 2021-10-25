<template>
  <div class="footer-wrapper">
    <div class="footer-box">
      <div class="footer-header">
        <ParaHeader text="Будем рады видеть тебя в клубе"/>
      </div>

      <div class="vk-button">
        <a href="https://vk.com/ftmlclub" class="linkFTML" target="_blank">
          <button class="vk">
            <img src="../assets/png/VK.png" alt="VK">
            Вступить в группу, чтобы быть в курсе всех событий
          </button>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import ParaHeader from "@/components/ParaHeader";

export default {
  name: "Footer",
  components: {
    ParaHeader
  }
}
</script>

<style lang="scss">
.footer-wrapper {
  width: 1200px;
  height: 140px;
  background-color: #001134;

  .footer-box {
    padding-top: 23px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-right: 126px;
    padding-left: 127px;
  }

  .footer-header {
    width: 317px;
    text-align: left;
  }

  .vk {
    text-decoration: none;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    font-family: "Roboto Regular";
    font-size: 16px;
    width: 501px;
    height: 48px;
    border: inherit;
    border-radius: 23px;
    color: #ffffff;
    background-image: linear-gradient(to right, #C89AFC, #7C6AFA);
  }
  .linkFTML {
    text-decoration: none;
  }
}

@font-face {
  font-family: "Roboto Regular";
  src: url("../assets/fonts/Roboto-Regular.ttf");
}

</style>