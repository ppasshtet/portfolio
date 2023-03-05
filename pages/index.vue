<template>
  <div class="index">
    <div class="default">
      <Header />
      <Welcome />
      <div class="scroll-down">
        <div class="scroll-down__text">
          scroll down
        </div>
        <div class="scroll-down__icon">
          <img src="@/assets/images/scroll-down.svg" alt="">
        </div>
      </div>
      <Headline>
        <template #title>
          About me
        </template>
        <template #subtitle>
          My introducatio
        </template>
      </Headline>
      <About />
      <Headline>
        <template #title>
          Skills
        </template>
        <template #subtitle>
          My  technical level
        </template>
      </Headline>
      <Knowledge />
      <Headline>
        <template #title>
          Portfolio
        </template>
        <template #subtitle>
          My portfolio works in other project
        </template>
      </Headline>
      <CarouselSlider />
      <Headline>
        <template #title>
          Resume
        </template>
        <template #subtitle>
          My resume on Linkedin and HeadHanter
        </template>
      </Headline>
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>

<style lang="scss">
  .index {
    padding: 20px 150px;
    background: $background;
  }
  .scroll-down {
    padding-top: 40px;
    font-family: "DMSansRegular";
    font-size: 12px;
    line-height: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .scroll-down__text {
    padding-right: 10px;
  }
  .scroll-down__icon {
    height: 16px;
    width: 16px;

  }
</style>
