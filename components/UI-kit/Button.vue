<template>
  <a v-if="telegram" class="button" :href="'https://t.me/cazacow'" target="_blank">
    <div class="button-text">
      <slot />
    </div>
    <div class="button-icon">
      <slot name="icon" />
    </div>
  </a>
  <a v-else-if="document" class="button" href="/img/kazakov.pdf" download="KazakovPavel">
    <div class="button-text">
      <slot />
    </div>
    <div class="button-icon">
      <slot name="icon" />
    </div>
  </a>
</template>

<script>
export default {
  props: {
    telegram: {
      type: Boolean,
      default: false
    },
    document: {
      type: Boolean,
      default: false
    }
  }
}
</script>

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
