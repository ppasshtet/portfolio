<template>
  <div class="resume">
    <div class="resume-headhunter">
      <a href="https://hh.ru/resume/8c72bd94ff08b9ba240039ed1f3550485a467a" />
      <ResumeLink>
        <template #icon>
          <img src="@/static/img/headHunter.png" alt="">
        </template>
        <template #name>
          HeadHunter
        </template>
      </ResumeLink>
    </div>
    <div class="resume-linkedin">
      <ResumeLink>
        <template #icon>
          <img src="@/assets/images/linkedin.svg" alt="">
        </template>
        <template #name>
          Linkedin
        </template>
      </ResumeLink>
    </div>
  </div>
</template>

<style lang="scss">
.resume{
    padding-top: 100px;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

</style>
