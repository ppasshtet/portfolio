<template>
  <div class="carousel">
    <carousel
      :autoplay="false"
      :nav="false"
      :loop="true"
      :items="1"
    >
      <img src="@/static/png/discordHunter.png">
    </carousel>
  </div>
</template>

<script>

import carousel from 'vue-owl-carousel'

export default {
  components: { carousel }
}

</script>

<style lang="scss">
.carousel {
  padding-top: 40px;
}
</style>
