<template>
    <header>
        <div class="container">
            <HeaderLeft></HeaderLeft>
            <HeaderRight></HeaderRight>
        </div>

    </header>
</template>

<script>
import HeaderLeft from './header-left/HeaderLeft';
import HeaderRight from './header-right/HeaderRight';

export default {
    name: "BaseHeader",
    components: { HeaderLeft, HeaderRight }
}
</script>

<style  lang="scss" scoped>
header {
    overflow: hidden;
    position: absolute;
    left: 50%;
    top: 15px;
    z-index: 1;
    transform: translateX(-50%);
    width: 100%;

    .container {
        display: flex;
        align-items: center;
        justify-content: space-between;
       
    }


}
</style>