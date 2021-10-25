<template>
  <div class="wrapper">
    <div class="header">
      <div class="logo">
        <div class="logo-text">
          <ul class="FTML">
            <li class="F"><img src="../assets/svg/F.svg" alt="F"></li>
            <li class="T"><img src="../assets/svg/T.svg" alt="T"></li>
            <li class="M"><img src="../assets/svg/M.svg" alt="M"></li>
            <li class="L"><img src="../assets/svg/L.svg" alt="L"></li>
          </ul>
        </div>
        <div class="logo-pic">
          <object type="image/svg+xml" class="light" :data=this.logo></object>
        </div>
      </div>

      <Menu/>

    </div>

  </div>

</template>


<script>
import Menu from "./Menu"

export default {
  name: "header",
  components: {
    Menu
  },
  data() {
    return{
      F: require("../assets/svg/F.svg"),
      T: require("../assets/svg/T.svg"),
      M: require("../assets/svg/M.svg"),
      L: require("../assets/svg/L.svg"),
      logo: require("../assets/svg/Full.svg"),
      back1: require("../assets/svg/Vector_6.svg")
    }
  }
}
</script>

<style lang="scss">
.wrapper {
  height: 65px;
  position: relative;


  .header{
    padding-top: 30px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
  }


  .logo-text {
    width: 40px;
    padding-left: 125px;
    display: flex;
    justify-content: center;



    .FTML {
      display: flex;

      li {
        list-style-type: none;
        padding-left: 1px;
      }

    }
  }

  .logo-pic {
    width: 40px;
    height: 34px;
    margin-left: 125px;

  }
}

</style>