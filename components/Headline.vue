<template>
  <div class="headline">
    <div class="headline-main">
      <slot name="title" />
    </div>
    <div class="headline-subtitle">
      <slot name="subtitle" />
    </div>
  </div>
</template>

<style lang="scss">
    .headline {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: 100px;
    }
    .headline-main {
        font-family: "ManropeBold";
        font-size: 30px;
        line-height: 40px;
        color: $black;
    }
    .headline-subtitle {
        font-family: "DMSansMedium";
        font-size: 10px;
        line-height: 18px;
        color: $brand-light;
        padding-top: 5px;
    }
</style>
