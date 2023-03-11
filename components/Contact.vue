<template>
  <div class="contact">
    <a href="mailto:quint905@gmail.com">
      <ContactBlock
        :info="true"
      >
        <template #icon>
          <img src="@/assets/images/mail.svg" alt="">
        </template>
        <template #name>
          Email
        </template>
        <template #contact>
          quint905@gmail.com
        </template>
      </ContactBlock>
    </a>
    <a :href="'https://wa.me/79111783619'" target="_blank">
      <ContactBlock
        :info="true"
      >
        <template #icon>
          <img src="@/assets/images/whatsapp.svg" alt="">
        </template>
        <template #name>
          WhatsApp
        </template>
        <template #contact>
          +79111783619
        </template>
      </ContactBlock>
    </a>
    <a :href="'https://t.me/cazacow'" target="_blank">
      <ContactBlock
        :info="true"
      >
        <template #icon>
          <img src="@/assets/images/telegram.svg" alt="">
        </template>
        <template #name>
          Telegram
        </template>
        <template #contact>
          @cazacow
        </template>
      </ContactBlock>
    </a>
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
