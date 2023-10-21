<template>
  <div
    class="header text"
    :class="{'headerScroll': headerScroll}"
  >
    <div class="logo text--16">
      <Logo />
    </div>
    <div class="menu text--16">
      <NuxtLink class="link" to="">
        Home
      </NuxtLink>
      <NuxtLink v-scroll-to="{el: '#about', offset: -70}" class="link" to="">
        About
      </NuxtLink>
      <NuxtLink v-scroll-to="{el: '#skills', offset: 30}" class="link" to="">
        Skills
      </NuxtLink>
      <NuxtLink v-scroll-to="{el: '#way', offset: -70}" class="link" to="">
        Way
      </NuxtLink>
      <NuxtLink v-scroll-to="{el: '#portfolio', offset: -70}" class="link" to="">
        Portfolio
      </NuxtLink>
      <NuxtLink v-scroll-to="'#contact'" class="link" to="">
        Contact
      </NuxtLink>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      headerScroll: false
    }
  },
  mounted: function () {
    this.checkScrollPosition()
    window.addEventListener('scroll', this.checkScrollPosition)
  },
  methods: {
    checkScrollPosition () {
      this.headerScroll = window.pageYOffset > 10
    }
  }
}
</script>

<style lang="scss" scoped>
  .header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    height: 50px;
    z-index: 1;
    transition: all 0.3s ease;
    top: 0;
    padding: 0px 120px;
    position: fixed;
    transition: all 0.3s ease;
  }
  .headerScroll {
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    background: $border;
    transition: all 0.3s ease;
    border-radius: 0px 0px 10px 10px;
    opacity: .95;
  }
  .menu:last-child {
    padding-right: 0px;
  }
  .link{
    color: $brand;
    transition: all 0.3s ease;
    padding-left: 40px;
  }
  .link:hover {
    opacity: 0.7;
  }
  .logo {
    font-family: "ManropeBold";
    color: $black;
  }
</style>
