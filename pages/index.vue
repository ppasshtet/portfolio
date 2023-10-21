<template>
  <div class="index">
    <Header />
    <div class="container">
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
      <Welcome />
      <ScrollDown />
      <About />
      <Skills />
      <Way />
      <Headline
        id="portfolio"
        :title="'Portfolio'"
        :subtitle="'My portfolio works in other project'"
      />
      <CarouselSlider />
      <Headline
        id="contact"
        :title="'Contact me'"
        :subtitle="'Get in touch'"
      />
      <Contact />
    </div>
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

@media only screen and (max-width : 390px) {
  .index {
    padding: 10px 40px;
  }
}
</style>
