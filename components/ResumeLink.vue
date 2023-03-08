<template>
  <div class="resume-link">
    <div class="resume-icon">
      <slot name="icon" />
    </div>
    <div class="resume-name">
      <slot name="name" />
    </div>
    <div class="resume-contact text text--12">
      <slot name="contact" />
    </div>
    <div class="resume-info">
      <div class="resume-info__text">
        view more
      </div>
      <div class="resume-info__icon">
        <img src="@/assets/images/view-more.svg" alt="">
      </div>
    </div>
  </div>
</template>

<style lang="scss">

.resume-link {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    padding: 15px;
    border: 1px solid $gray;
    border-radius: 15px;
    height: 150px;
    width: 450px;
}
.resume-icon {
    width: 48px;
    height: 48px;
}
.resume-name {
    font-family: "DMSansRegular";
    font-size: 16px;
    line-height:20px;
    color: $brand;
}
.resume-info {
    font-family: "DMSansRegular";
    font-size: 14px;
    line-height: 16px;
    color: $gray;
    display: flex;
    flex-direction: row;
}
.resume-info__text {
    padding-right: 10px;
}
.resume-info__icon {
    height: 20px;
    width: 20px;
}
</style>
