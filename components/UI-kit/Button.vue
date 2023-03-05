<template>
    <div class="button">
        <div class="button-text">
            <slot />
        </div>
        <div class="button-icon">
            <slot name="icon" />
        </div>
    </div>
</template>

<style lang="scss">
    .button {
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: fit-content;
        height: 40px;
        background-color: $black;
        border-radius: 10px;
        color: $white;
        padding: 10px 30px;
    }
    .button-text {
        font-family: "DMSansBold";
        font-size: 14px;
        line-height: 20px;
        background-color: $black;
        padding-right: 10px;
    }
    .button-icon {
        width: 25px;
        height: 25px;
    }
</style>