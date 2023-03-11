<template>
  <div class="footer">
    <div class="footer-logo">
      <Logo />
    </div>
    <div class="footer-info text--12">
      All right reserved. @cazacow 2023.
    </div>
  </div>
</template>

<style lang="scss">
.footer {
    margin-top: 100px;
    width: 100%;
    height: 60px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
}
.footer-logo{
  font-size: 30px;
  line-height: 34px;
}
.footer-info {
    color: $brand-light;
}
</style>
