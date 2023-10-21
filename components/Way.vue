<template>
  <div id="way" class="way">
    <Headline
      :title="'My way'"
      :subtitle="'My professional way in other project'"
    />
    <div class="way-block">
      <div
        v-for="(wayArray, wayArrayId) in wayArrays"
        :key="wayArrayId"
        class="way-block__info"
      >
        <div class="info">
          <WorkBlock
            :title="wayArray.title"
            :subtitle="wayArray.subtitle"
            :location="wayArray.location"
            :date="wayArray.date"
            :leftPosition="wayArray.position"
            @click="showModal = true"
          />
        </div>
      </div>
    </div>
    <BlockModal v-show="showModal" @close-modal="showModal = false" />
  </div>
</template>

<script>
export default {
  data () {
    return {
      wayArrays: [
        {
          title: 'Freelance',
          subtitle: 'Frontend Web Developer',
          location: 'Montenegro',
          date: 'October 2022 — March 2023',
          position: true,
          num: 0,
          info: ['1', '2', '3']
        },
        {
          title: 'Infinity Girls',
          subtitle: 'Frontend Web | Blockchain Developer',
          location: 'Saint-Petersburg',
          date: 'February 2022 — May 2022',
          position: false,
          num: 1,
          info: ['4', '5', '6']
        },
        {
          title: 'Enigma Robotics',
          subtitle: 'Frontend Web Developer',
          location: 'Saint-Petersburg',
          date: 'September 2020 — March 2022',
          position: true,
          num: 2,
          info: ['7', '8', '9']
        },
        {
          title: 'Bekary 85',
          subtitle: 'Frontend Web Developer',
          location: 'Saint-Petersburg',
          date: 'September 2019 — August 2020',
          position: false,
          num: 3,
          info: ['10', '11', '12']
        },
        {
          title: 'Bonch Dev',
          subtitle: 'Frontend Web Developer',
          location: 'Saint-Petersburg',
          date: 'October 2018 — June 2019',
          position: true,
          num: 4,
          info: ['13', '14', '15']
        }
      ],
      showModal: false
    }
  }
}
</script>

<style lang="scss">
.way-block{
  width: 100%;
  height: auto;
  position: relative;
  margin-top: 100px;
}
.way-block::before{
  content: "";
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 1px;
  height: 100%;
  background: $gray;
}
.way-block__info {
  height: 150px;
  width: 50%;
}
.way-block__info::before {
  content: "";
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 15px;
  height: 15px;
  border-radius: 15px;
  background: $gray;
}
.way-block__info:nth-child(even){
  margin-left: auto;
  padding-left: 40px;
}
.way-block__info:nth-child(odd) {
  .info {
    position: relative;
  }
}
.way-block__info:last-child::after {
  content: "";
  position: absolute;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 15px;
  height: 15px;
  border-radius: 15px;
  background: $gray;
}
.info {
  width: auto;
  height: 150px;
}
</style>
