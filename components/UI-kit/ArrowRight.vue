<template>
  <div class="arrow">
    <div class="arrow-animate" />
  </div>
</template>

<style lang="scss" scoped>
.arrow {
    cursor: pointer;
    position: relative;
    width: auto;
    height: 20px;
}
.arrow-animate {
    position: relative;
    top: 10px;
    width: 11px;
    height: 1px;
    background-color: $brand;
    box-shadow: 0 3px 5px rgba(0, 0, 0, .2);
    left:0;
    display: block;

    animation: arrow-animate 2s linear infinite;
}
.arrow-animate::after {
    content: '';
    position: absolute;
    width: 5px;
    height: 1.25px;
    top: -1.5px;
    right: -2px;
    background-color: $brand;
    transform: rotate(45deg);
}
.arrow-animate::before {
    content: '';
    position: absolute;
    width: 5px;
    height: 1.25px;
    top: 1.5px;
    right: -2px;
    background-color: $brand;
    box-shadow: 0 3px 5px rgba(0, 0, 0, .2);
    transform: rotate(-45deg);
}
    @keyframes arrow-animate {
    0% {
        left: 10px;
    }
    50% {
        left: 20px;
    }
    100% {
        left: 10px;
    }
    }

</style>
