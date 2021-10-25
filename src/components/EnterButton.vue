<template>
  <div class="enter-button-box">
    <a href="https://vk.com/ftmlclub" target="_blank">
      <button class="enter-button">
        Вступить
      </button>
    </a>
  </div>
</template>

<script>
export default {
  name: "EnterButton"
}
</script>

<style lang="scss">
.enter-button-box {
  padding-left: 135px;
  display: flex;
  justify-content: flex-start;
}

.enter-button {
  width: 279px;
  height: 50px;
  border-radius: 50px;
  border: inherit;
  background: linear-gradient(to right, #C89AFC, #7C6AFA);
  color: #FFFFFF;
  font-size: 16px;
}

</style>