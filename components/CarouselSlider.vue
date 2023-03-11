<template>
  <div class="carouselSlider">
    <carousel
      class="carousel"
      :perPage="1"
      :loop="true"
      :autoplay="true"
      :autoplayTimeout="4000"
      paginationColor="#B6B6B6"
    >
      <slide>
        <img src="@/static/img/discordLink.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/discordSettings.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/webAio.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/dashboardEnigma.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/infinityGirls.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/heroesCity.svg" alt="">
      </slide>
      <slide>
        <img src="@/static/img/hackaton.svg" alt="">
      </slide>
    </carousel>
  </div>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'

export default {
  components: {
    Carousel,
    Slide
  }
}
</script>

<style lang="scss">
.carouselSlider {
  padding-top: 40px;
  display: flex;
  justify-content: center;

}
.carousel {
  width: 900px;
  height: auto;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
