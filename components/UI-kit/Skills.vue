<template>
  <div class="skills">
    <div class="skills-icon">
      <slot name="icon" />
    </div>
    <div class="skills-name">
      <slot name="name" />
    </div>
    <div class="skills-info">
      <slot name="info" />
    </div>
  </div>
</template>

<style lang="scss">
    .skills {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
        padding: 15px;
        border: 2px solid $gray;
        border-radius: 15px;
        height: 150px;
        width: 180px;
    }
    .skills-name {
        font-family: "DMSansRegular";
        font-size: 16px;
        line-height:20px;
        color: $brand;
    }
    .skills-info {
        font-family: "DMSansRegular";
        font-size: 14px;
        line-height: 16px;
        color: $gray;
    }
</style>
