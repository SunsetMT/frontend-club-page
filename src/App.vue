<template>
  <div id="app">
    <UpWrapper/>
  </div>
</template>

<script>
import UpWrapper from "@/components/UpWrapper";

export default {
  name: 'App',
  components: {
    UpWrapper
  },
  data() {
    return {
      back1: require("/src/assets/svg/Vector_6.svg"),
      back2: require("/src/assets/svg/Vector_5.svg"),
    }
  }
}
</script>

<style>


#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0;
  max-width: 1200px;
  position: relative;
}




ul {
  padding: 0;
  margin: 0;
}

body {
  margin: 0;
}
</style>
