<template>
  <div class="index">
    <transition name="fade">
      <div v-if="buttonShow" class="buttonUp" @click="click">
        <div class="buttonUp-text">
          Upstairs
        </div>
        <div class="buttonUp-icon">
          <img src="@/assets/images/scroll-up.svg" alt="">
        </div>
      </div>
    </transition>
    <Header />
    <Welcome />
    <ScrollDown />
    <Headline id="about">
      <template #title>
        About me
      </template>
      <template #subtitle>
        My introducatio
      </template>
    </Headline>
    <About />
    <Headline id="skills">
      <template #title>
        Skills
      </template>
      <template #subtitle>
        My technical level
      </template>
    </Headline>
    <Knowledge />
    <Headline id="way">
      <template #title>
        My way
      </template>
      <template #subtitle>
        My professional way in other project
      </template>
    </Headline>
    <Way />
    <Headline id="portfolio">
      <template #title>
        Portfolio
      </template>
      <template #subtitle>
        My portfolio works in other project
      </template>
    </Headline>
    <CarouselSlider />
    <Headline id="contact">
      <template #title>
        Contact me
      </template>
      <template #subtitle>
        Get in touch
      </template>
    </Headline>
    <Contact />
    <Footer />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data () {
    return {
      buttonShow: false
    }
  },
  mounted: function () {
    this.checkScrollPosition()
    window.addEventListener('scroll', this.checkScrollPosition)
  },
  methods: {
    checkScrollPosition () {
      this.buttonShow = window.pageYOffset > 10
    },
    click () {
      scroll({
        top: 0,
        behavior: 'smooth'
      })
    }
  }
}
</script>

<style lang="scss">
.index {
  padding: 10px 150px;
  background: $background;
}
.buttonUp{
  position: fixed;
  right: 35px;
  bottom: 35px;
  background-color: $black;
  color: $white;
  border-radius: 10px;
  padding:  10px 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.3s ease;
  z-index: 9999;
}
.buttonUp:hover {
  opacity: 0.7;
  cursor: pointer;
}
.buttonUp-text {
  padding-right: 5px;
  font-family: "DMSansBold";
  font-size: 14px;
  line-height: 20px;
  padding-right: 10px;
}
.buttonUp-icon {
  width: 16px;
  height: 16px;
  color: $white;
}
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to {
  opacity: 0;
}
</style>
