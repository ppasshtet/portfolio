<template>
  <div class="work-block text">
    <div class="work-block__title text--14">
      <slot name="title" />
    </div>
    <div class="work-block__subtitle text--14">
      <slot name="subtitle" />
    </div>
    <div class="work-block__location text--14">
      <slot name="location" />
    </div>
    <div class="work-block__date text--12">
      <div class="date-icon">
        <img src="@/assets/images/date.svg" alt="">
      </div>
      <div class="date-text">
        <slot name="date" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.work-block {
    display: flex;
    flex-direction: column;
}
.work-block__title {
  color: $brand !important;
}
.work-block__date {
    display: flex;
    align-items: center;
}
.date-icon {
  display: flex;
  justify-content: center;
  >img {
    width: 20px;
    height: 20px;
  }
}
.date-text {
  padding-left: 10px;
}
</style>
