<template>
  <div class="welcome">
    <div class="welcome-left">
      <div class="welcome-logo">
        <Logo />
      </div>
      <div class="welcome-info">
        <div class="info-line" />
        <div class="info-text">
          Web | Blockchain Developer
        </div>
      </div>
      <div class="welcome-text">
        I’m Web | Blockchain Developer in Montenegro, and I’m very passionate
        and dedicated to my work
      </div>
      <div class="welcome-button">
        <Button>
          say Hello
          <template #icon>
            <img src="@/assets/images/send.svg" alt="">
          </template>
        </Button>
      </div>
    </div>
    <div class="welcome-right">
      <div class="welcome-photo">
        <Avatar />
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
    .welcome {
        font-family: "ManropeBold";
        font-size: 24px;
        line-height: 18px;
        display: flex;
        justify-content: space-between;
    }
    .welcome-left {
        display: flex;
        flex-direction: column;
    }
    .welcome-logo {
        font-size: 50px;
        line-height: 60px;
    }
    .welcome-info{
        font-family:  "DMSansMedium";
        font-size: 24px;
        line-height: 30px;
        color: $brand;
        display: flex;
        align-items: center;
        padding-top: 30px;
    }
    .info-line {
        width: 72px;
        height: 0px;
        border: 0.5px solid $black;

    }
    .info-text {
        padding-left: 20px;
    }
    .welcome-text {
        font-family:  "DMSansMedium";
        font-size: 16px;
        line-height: 24px;
        color: $brand-light;
        padding: 40px 200px 0px 0px;
    }
    .welcome-button {
        padding-top: 40px;
    }
</style>
