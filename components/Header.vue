<template>
    <div class="header">
        <div class="header-position">
            <div class="logo">
                <Logo />
            </div>
            <div class="menu">
                <Menu />
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .header {
        height: 100px;
        width: 100%;

    }
    .header-position {
        display: flex;
        justify-content: space-between;
        flex-direction:row;
        align-items: center;

    }
    .logo {
        font-size: 20px;
        line-height: 24px;
    }
    .menu {
       
    }
</style>