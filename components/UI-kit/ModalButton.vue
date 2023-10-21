<template>
  <div class="button" @click="$emit('click')">
    <div class="button-text">
      close It
    </div>
    <div class="button-icon">
      <img src="@/assets/images/send.svg" alt="">
    </div>
  </div>
</template>

<style lang="scss">
.button {
  display: flex;
  justify-content: space-around;
  align-items: center;
  width: fit-content;
  height: 40px;
  background-color: $black;
  border-radius: 10px;
  color: $white;
  padding: 10px 30px;
  transition: all 0.3s ease;
}
.button:hover{
  opacity: 0.7;
  cursor: pointer;
}
.button-text {
  font-family: "DMSansBold";
  font-size: 14px;
  line-height: 20px;
  padding-right: 10px;
}
.button-icon {
  width: 25px;
  height: 25px;
}
</style>
