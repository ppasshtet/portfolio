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
        <Button
          :telegram="true"
        >
          say Hello
          <template #icon>
            <img src="@/assets/images/send.svg" alt="">
          </template>
        </Button>
      </div>
      <div class="welcome-link">
        <div class="welcome-link__linkedin">
          <a :href="'https://www.linkedin.com/in/pavel-kazakov-76359a233/'" target="_blank">
            <svg width="30" height="30" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M0 7.17617C0 11.1395 3.21288 14.3523 7.17617 14.3523C11.1395 14.3523 14.3523 11.1395 14.3523 7.17617C14.3523 3.21288 11.1395 0 7.17617 0C3.21288 0 0 3.21288 0 7.17617Z" fill="black" />
              <path d="M5.20273 10.7642H3.67779V5.96518H5.20273V10.7642ZM4.44026 5.29241C3.9469 5.29241 3.58809 4.93361 3.58809 4.44024C3.58809 3.94688 3.99175 3.58807 4.44026 3.58807C4.93362 3.58807 5.29243 3.94688 5.29243 4.44024C5.29243 4.93361 4.93362 5.29241 4.44026 5.29241ZM10.7643 10.7642H9.23933V8.16288C9.23933 7.40041 8.92536 7.17616 8.47685 7.17616C8.02834 7.17616 7.57983 7.53497 7.57983 8.20773V10.7642H6.0549V5.96518H7.49013V6.63795C7.62468 6.32399 8.16289 5.83063 8.92536 5.83063C9.77753 5.83063 10.6746 6.32399 10.6746 7.80407V10.7642H10.7643Z" fill="white" />
            </svg>
          </a>
        </div>
        <div class="welcome-link__headHunter">
          <a :href="'https://hh.ru/resume/8c72bd94ff08b9ba240039ed1f3550485a467a'" target="_blank">
            <svg viewBox="0 0 180 180" fill="none" xmlns="http://www.w3.org/2000/svg">
              <circle cx="90" cy="90" r="90" fill="black" />
              <path d="M57.1986 55V82.0165C61.1258 77.1122 65.8334 74.6435 71.2929 74.6435C74.1048 74.6435 76.6229 75.2061 78.8819 76.3213C81.1472 77.4299 82.8407 78.8529 83.9844 80.5803C85.1345 82.3243 85.9117 84.2337 86.3319 86.3383C86.7489 88.4331 86.9574 91.6927 86.9574 96.1138V125H74.7557V98.9829C74.7557 93.8205 74.5345 90.551 74.0701 89.1611C73.6349 87.7996 72.7717 86.633 71.6215 85.8519C70.4462 85.0213 68.9834 84.6109 67.2172 84.6109C65.1952 84.6109 63.3817 85.1404 61.8051 86.1927C60.1938 87.2517 59.0374 88.8335 58.3044 90.9481C57.5588 93.066 57.186 96.1932 57.1986 100.333L57.186 125H45V55H57.2018M105.244 55V82.0165C109.175 77.1122 113.879 74.6435 119.335 74.6435C122.138 74.6435 124.675 75.2061 126.937 76.3213C129.193 77.4299 130.886 78.8529 132.024 80.5803C133.172 82.3127 133.97 84.2719 134.371 86.3383C134.791 88.4331 135 91.6927 135 96.1138V125H122.811V98.9829C122.811 93.8205 122.58 90.551 122.116 89.1611C121.681 87.7977 120.815 86.6305 119.661 85.8519C118.498 85.0213 117.023 84.6109 115.257 84.6109C113.238 84.6109 111.424 85.1404 109.844 86.1927C108.255 87.2517 107.093 88.8335 106.35 90.9481C105.617 93.066 105.244 96.1932 105.244 100.333V125H93.0583V55H105.244Z" fill="#FEFEFE" />
            </svg>
          </a>
        </div>
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
        justify-content: space-between;
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
        padding: 0px 200px 0px 0px;
    }
    .welcome-link {
      display: flex;
    }
    .welcome-link__headHunter {
      width: 30px;
      height: 30px;
      left: 15px;
      transform: translateX(15px);
      > svg {
        width: 30px;
        height: 30px;
      }
    }
</style>
