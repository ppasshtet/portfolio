<template>
  <div class="about">
    <div class="about-image">
      <img src="@/static/img/bear-2.png" alt="">
    </div>
    <div class="about-info">
      <div class="about-info__icons">
        <Skills>
          <template #icon>
            <img src="@/assets/images/dash.svg" alt="">
          </template>
          <template #name>
            Experience
          </template>
          <template #info>
            3+ years
          </template>
        </Skills>
        <Skills>
          <template #icon>
            <img src="@/assets/images/comp.svg" alt="">
          </template>
          <template #name>
            Completed
          </template>
          <template #info>
            8+ projects
          </template>
        </Skills>
        <Skills>
          <template #icon>
            <img src="@/assets/images/terminal.svg" alt="">
          </template>
          <template #name>
            Technology
          </template>
          <template #info>
            10+ skills
          </template>
        </Skills>
      </div>
      <div class="about-info__text">
        Blockchain | Frontend developer, I create web pages user interface, I have years of experience. I also love Web 3, I think it has a great future
      </div>
      <div class="about-info__button">
        <Button
          :document="true"
        >
          Download resume
          <template #icon>
            <img src="@/assets/images/file.svg" alt="">
          </template>
        </Button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
    .about {
        display: flex;
        justify-content: space-between;
        padding-top: 40px;
    }
    .about-image {
        width: 320px;
        height: 300px;
        border: 10px solid $border;
        border-radius: 20px;
        overflow: hidden;
    }
    .about-info {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        width: 60%;
    }
    .about-info__icons {
        display: flex;
        justify-content: space-between;
    }
    .about-info__text {
        font-family: "DMSansRegular";
        font-size: 16px;
        line-height: 20px;
        color: $brand-light;
    }
</style>
