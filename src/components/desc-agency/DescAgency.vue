<template>
    <div>
        <div class="logo">
            <img src="../../assets/img/medical_logo_1x_dark.png" alt="">
        </div>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolorum nihil dignissimos repellendus optio
            incidunt dolores, molestiae unde ab consequatur sunt obcaecati ducimus, dolor nisi minus labore
            corporis, provident voluptate quaerat!</p>
        <hr>
        <h3>LEARN MORE ABOUT US</h3>
        <div class="social">
            <i class="fa-brands fa-facebook-square"></i>
            <i class="fa-brands fa-twitter-square"></i>
            <i class="fa-brands fa-youtube-square"></i>
            <i class="fa-brands fa-instagram-square"></i>
        </div>
    </div>
</template>

<script>
export default {
    name: 'DescAgency'
}
</script>

<style lang="scss" scoped>
div:first-child {

    p {
        margin-top: 10px;
        line-height: 30px;
    }

    & .social {
        margin-top: 30px;

        svg {
            font-size: 30px;
            margin-right: 10px;
            transition: 0.25s;


            &:hover {
                transition: 0.25s;
                cursor: pointer;
                transform: scale(1.5);
            }
        }
    }

    hr {
        width: 100%;
        margin-bottom: 0;
    }
}
</style>