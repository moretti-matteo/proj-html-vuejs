<template>
  <div>
    <a href="#head"><i class="fa-solid fa-chevron-up"></i></a>
  </div>
</template>

<script>
export default {
    name:'BackUp'
}
</script>

<style lang="scss" scoped>
    div{
        height: 30px;
        width: 30px;
        background-color: var(--color-lightdark);
        position: fixed;
        left:90%;
        bottom:0;
        transform: translateX(-90%);
        text-align: center;

        a{
            line-height: 30px;
            color:white;
            text-decoration: none;

            svg{
                font-size: 15px;
            }
        }
    }
</style>