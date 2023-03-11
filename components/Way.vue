<template>
  <div class="way">
    <div class="way-block">
      <div class="way-block__info">
        <WorkBlock>
          <template #title>
            Freelance
          </template>
          <template #subtitle>
            Frontend Web Developer
          </template>
          <template #location>
            Montenegro
          </template>
          <template #date>
            October 2022 — March 2023
          </template>
        </WorkBlock>
      </div>
    </div>
    <div class="way-block">
      <div class="way-block__info">
        <WorkBlock>
          <template #title>
            Infinity Girls
          </template>
          <template #subtitle>
            Frontend Web | Blockchain Developer
          </template>
          <template #location>
            Saint-Petersburg
          </template>
          <template #date>
            February 2022 — May 2022
          </template>
        </WorkBlock>
      </div>
    </div>
    <div class="way-block">
      <div class="way-block__info">
        <WorkBlock>
          <template #title>
            Enigma Robotics
          </template>
          <template #subtitle>
            Frontend Web Developer
          </template>
          <template #location>
            Saint-Petersburg
          </template>
          <template #date>
            September 2020 — March 2022
          </template>
        </WorkBlock>
      </div>
    </div>
    <div class="way-block">
      <div class="way-block__info">
        <WorkBlock>
          <template #title>
            Bekary 85
          </template>
          <template #subtitle>
            Frontend Web Developer
          </template>
          <template #location>
            Saint-Petersburg
          </template>
          <template #date>
            September 2019 — August 2020
          </template>
        </WorkBlock>
      </div>
    </div>
    <div class="way-block">
      <div class="way-block__info">
        <WorkBlock>
          <template #title>
            Bonch Dev
          </template>
          <template #subtitle>
            Frontend Web Developer
          </template>
          <template #location>
            Saint-Petersburg
          </template>
          <template #date>
            October 2018 — June 2019
          </template>
        </WorkBlock>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.way{
  width: 100%;
  height: auto;
  position: relative;
  margin-top: 100px;
}
.way::before{
  content: "";
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 1px;
  height: 100%;
  background: $gray;
}
.way-block {
  height: 150px;
  width: 50%;
}
.way-block::before {
  content: "";
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 15px;
  height: 15px;
  border-radius: 15px;
  background: $gray;
}
.way-block:nth-child(even){
  margin-left: auto;
  padding-left: 5%;
}
.way-block:nth-child(odd) {
  padding-left: 27%;
}
.way-block:last-child::after {
  content: "";
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 15px;
  height: 15px;
  border-radius: 15px;
  background: $gray;
}
.way-block__info {
  width: auto;
  height: 150px;
}
</style>
