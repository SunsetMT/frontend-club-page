<template>
  <div class="card-wrapper">
    <div class="card">
      <div class="card-text">
        Клуб будет полезен студентам, которые хотят чего-то большего. Если ты готов развивать свои hard skills в
        клиентской стороне пользовательского интерфейса, то тебе к нам
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MotivationCard"
}
</script>

<style lang="scss">
.card-wrapper {
  display: flex;
  justify-content: center;
  margin-bottom: 43px;

  .card {
    width: 706px;
    height: 114px;
    margin-top: 61px;
    border-radius: 11px;
    border: inherit;
    background: linear-gradient(to right, #C89AFC, #7C6AFA);
    .card-text {
      font-family: "Raleway Regular";
      display: flex;
      text-align: center;
      color: #ffffff;
      font-size: 16px;
      line-height: 140%;
      margin: 24px 16px 24px 16px;
    }
  }

}


@font-face {
  font-family: "Raleway Regular";
  src: url("../assets/fonts/Raleway-Regular.ttf");
}

</style>