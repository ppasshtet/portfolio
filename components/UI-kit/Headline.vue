<template>
  <div class="headline">
    <div class="headline-title">
      <h2>{{ title }}</h2>
    </div>
    <div class="headline-subtitle">
      <h6>{{ subtitle }}</h6>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    subtitle: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss">
.headline {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 100px;
}
</style>
