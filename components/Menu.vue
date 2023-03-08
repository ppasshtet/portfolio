<template>
  <div class="menu">
    <NuxtLink class="link" to="">
      Home
    </NuxtLink>
    <NuxtLink class="link" to="">
      About
    </NuxtLink>
    <NuxtLink class="link" to="">
      Service
    </NuxtLink>
    <NuxtLink class="link" to="">
      Skills
    </NuxtLink>
    <NuxtLink class="link" to="">
      Blog
    </NuxtLink>
    <NuxtLink class="link" to="">
      Contact
    </NuxtLink>
  </div>
</template>

<script>

export default {

}
</script>

<style lang="scss" scoped>
.menu {
  font-family: "DMSansRegular";
  font-size: 14px;
  line-height: 18px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
.link{
  color: $brand;
  padding-left: 70px;
  display: flex;
  justify-content: center;
  transition: all 0.3s ease;
}
.link:hover {
  color: $gray;
}
</style>
