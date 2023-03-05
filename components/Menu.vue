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
    }
    .link{
        color: $brand;
    }
</style>
