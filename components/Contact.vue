<template>
  <div class="contact">
    <ResumeLink>
      <template #icon>
        <img src="@/assets/images/mail.svg" alt="">
      </template>
      <template #name>
        Email
      </template>
      <template #contact>
        quint905@gmail.com
      </template>
    </ResumeLink>
    <ResumeLink>
      <template #icon>
        <img src="@/assets/images/whatsapp.svg" alt="">
      </template>
      <template #name>
        WhatsApp
      </template>
      <template #contact>
        +79111783619
      </template>
    </ResumeLink>
    <ResumeLink>
      <template #icon>
        <img src="@/assets/images/telegram.svg" alt="">
      </template>
      <template #name>
        Telegram
      </template>
      <template #contact>
        @cazacow
      </template>
    </ResumeLink>
  </div>
</template>

<style lang="scss">
.contact{
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding-top: 40px;
}
</style>
