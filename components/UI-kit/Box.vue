<template>
  <div class="box">
    <div class="box-icon">
      <slot name="icon" />
    </div>
    <div class="box-name">
      <h3>{{ name }}</h3>
    </div>
    <div class="box-info text text--14">
      <h4>{{ info }}</h4>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      type: String,
      default: ''
    },
    info: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss">
.box {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  padding: 15px;
  border: 1px solid $gray;
  border-radius: 15px;
  height: 150px;
  width: 180px;
}
</style>
