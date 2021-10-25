<template>
  <div class="menu-wrapper">
    <ul class="menu-el">
      <li><a href="#">Главная</a></li>
      <li><a href="#activity">Мероприятия</a></li>
      <li><a href="#mentors">Руководители</a></li>
      <li><a href="#participants">Участники</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Menu"
}
</script>

<style lang="scss">


.menu-wrapper{
  font-family: "Raleway Bold";
  padding-top: 20px;
  padding-right: 95px;
  color: #FFFFFF;

  .menu-el{
    display: flex;
    li{
      list-style-type: none;
      padding-right: 30px;
      a{
        color: #ffffff;
        text-decoration: none;
      }
    }
  }


  justify-content: flex-end;
}

@font-face {
  font-family: "Raleway Bold";
  src: url("../assets/fonts/Raleway-Bold.ttf");
}

</style>