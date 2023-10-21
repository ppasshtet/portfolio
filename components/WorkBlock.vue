<template>
  <div
    class="work-block text"
    :class="{'work-block__left': leftPosition}"
  >
    <div class="work-block__title text--14">
      {{ title }}
    </div>
    <div class="work-block__subtitle space text--14">
      {{ subtitle }}
    </div>
    <div class="work-block__location space text--14">
      {{ location }}
    </div>
    <div class="work-block__date space text--12">
      <div class="date-icon">
        <img src="@/assets/images/date.svg" alt="">
      </div>
      <div class="date-text">
        {{ date }}
      </div>
    </div>
    <div class="work-block__more">
      <div
        class="more-text text--14"
      >
        More info
      </div>
      <div class="more-arrow">
        <ArrowRight />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    subtitle: {
      type: String,
      default: ''
    },
    location: {
      type: String,
      default: ''
    },
    date: {
      type: String,
      default: ''
    },
    leftPosition: {
      type: Boolean,
      default: false
    }
  },
  data () {
    return {
      objWay: {}
    }
  }
  // methods: {
  //   defineBlockWay (objectOfWay) {
  //     console.log(objectOfWay)
  //     this.objWay = {}
  //     this.objWay = objectOfWay
  //     this.$modal.show('my-modal', this.objWay)
  //     console.log(this.objWay)
  //   }
  // }
}
</script>

<style lang="scss">
.work-block {
    display: flex;
    flex-direction: column;
    width: 300px;
    border: 1px solid $gray;
    border-radius: 10px;
    padding: 10px;
    cursor: pointer;
}
.work-block__left {
  position: absolute;
  right: 0;
  transform: translateX(-40px);
}
.work-block__title {
  color: $brand !important;
}
.space {
  padding-top: 4px;
}
.work-block__date {
    display: flex;
    align-items: center;
}
.date-icon {
  display: flex;
  justify-content: center;
  margin-left: -2px;
  >img {
    width: 20px;
    height: 20px;
  }
}
.date-text {
  padding-left: 10px;
}
.work-block__more {
  display: flex;
  align-items: center;
}
.more-text {
  color: $brand !important;
}
</style>
