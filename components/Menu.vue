<template>
  <div class="menu">
    <NuxtLink class="link" to="">
      Home
    </NuxtLink>
    <NuxtLink v-scroll-to="'#about'" class="link" to="">
      About
    </NuxtLink>
    <NuxtLink v-scroll-to="'#skills'" class="link" to="">
      Skills
    </NuxtLink>
    <NuxtLink v-scroll-to="'#way'" class="link" to="">
      Way
    </NuxtLink>
    <NuxtLink v-scroll-to="'#portfolio'" class="link" to="">
      Portfolio
    </NuxtLink>
    <NuxtLink v-scroll-to="'#contact'" class="link" to="">
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
  padding-left: 50px;
  display: flex;
  justify-content: center;
  transition: all 0.3s ease;
}
.link:hover {
  color: $gray;
}
</style>
