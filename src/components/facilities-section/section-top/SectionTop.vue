<template>
    <div class="section__top">
        <div class="container-sm">
            <div class="eye-logo">
                <img src="../../../assets/img/icon-7.png" alt="eye icon" />
            </div>
            <h1>TOUR OUR FACILITIES</h1>
            <hr />
            <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil autem
                aspernatur laboriosam cupiditate saepe magnam earum provident
                necessitatibus nesciunt ad, officiis voluptate est, quisquam amet
                culpa illo quia non blanditiis!
            </p>
            <button class="play"></button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'SectionTop'
}
</script>

<style lang="scss" scoped>
.section__top {
    background-image: url("../../../assets/img/paralax-bg-tour-facilities.jpg");
    height: 95vh;
    background-position: center;
    background-size: cover;
    text-align: center;
    color: var(--color-white);
    display: flex;
    align-items: center;

    & h1 {
        font-weight: 300;
    }

    & hr {
        width: 50%;
        margin: 20px auto;
        border: 1px solid var(--color-lightgrey);
        background-color: var(--color-lightgrey);
    }

    .play {
        height: 50px;
        width: 50px;
        border-radius: 50%;
        background-image: url("../../../assets/img/play-icon.png");
        background-position: center;
        background-size: cover;
        margin-top: 20px;
        border: none;
        transition: 0.25s;
    }

    .play:hover {
        cursor: pointer;
        transform: scale(1.2);
        transition: 0.25s;
    }
}
</style>