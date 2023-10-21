<template>
  <div class="footer">
    <div class="footer-logo">
      <h2><Logo /></h2>
    </div>
    <div class="footer-info">
      <h5>All right reserved. @cazacow 2023.</h5>
    </div>
  </div>
</template>

<style lang="scss">
.footer {
    transform: translateY(100px);
    width: 100%;
    height: 80px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    padding: 10px 120px;
}
.footer-logo{
  color: $black !important;
}
</style>
