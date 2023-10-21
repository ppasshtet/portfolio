<template>
  <div id="about" class="about">
    <Headline
      :title="'About me'"
      :subtitle="'My introducatio'"
    />
    <div class="about-content">
      <div class="about-content__image">
        <img src="@/static/img/bear-2.png" alt="">
      </div>
      <div class="about-content__info">
        <div class="info-blocks">
          <Box
            :name="'Experience'"
            :info="'3+ years'"
          >
            <template #icon>
              <img src="@/assets/images/dash.svg" alt="">
            </template>
          </Box>
          <Box
            :name="'Completed'"
            :info="'8+ projects'"
          >
            <template #icon>
              <img src="@/assets/images/comp.svg" alt="">
            </template>
          </Box>
          <Box
            :name="'Technology'"
            :info="'10+ skills'"
          >
            <template #icon>
              <img src="@/assets/images/terminal.svg" alt="">
            </template>
          </Box>
        </div>
        <div class="about-content__text">
          <h3>Blockchain | Frontend developer, I create web pages user interface, I have years of experience. I also love Web 3, I think it has a great future</h3>
        </div>
        <div class="about-content__button">
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
  </div>
</template>

<style lang="scss">
.about-content {
  display: flex;
  justify-content: space-between;
  margin-top: 40px;
}
.about-content__image {
  width: 320px;
  height: 300px;
  border: 10px solid $border;
  border-radius: 20px;
  overflow: hidden;
}
.about-content__info {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 60%;
}
.info-blocks {
  display: flex;
  justify-content: space-between;
}
</style>
