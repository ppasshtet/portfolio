<template>
  <div class="footer">
    <div class="footer-logo">
      <Logo />
    </div>
    <div class="footer-icon">
      <div class="footer-icon__linkedin footerImg">
        <img src="@/assets/images/linkedin.svg" alt="">
      </div>
      <div class="footer-icon__telegram footerImg">
        <img src="@/assets/images/telegram.svg" alt="">
      </div>
      <div class="footer-icon__email footerImg">
        <img src="@/assets/images/mail.svg" alt="">
      </div>
      <div class="footer-icon__whatsapp footerImg">
        <img src="@/assets/images/whatsapp.svg" alt="">
      </div>
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
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.footer-icon {
    display: flex;
    align-items: center;
    justify-content: space-around;
}
.footer-info {
    color: $brand-light;
}
</style>
