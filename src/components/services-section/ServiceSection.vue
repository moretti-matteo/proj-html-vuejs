<template>
    <section>
        <div class="container-md">
            <div class="container-sm">
                <div class="services-logo">
                    <img src="../../assets/img/icon-6.png" alt="">
                </div>
                <h1>OUR HEALTH SERVICES</h1>
                <hr noshade>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusantium reiciendis illo perferendis
                    corporis unde aspernatur consectetur inventore tempore modi, mollitia eveniet sapiente suscipit fuga
                    laudantium sint impedit non numquam consequatur?</p>
            </div>
            <div class="offered-services">
                <div class="service">
                    <img src="../../assets/img/icon-14.png" alt="">
                    <h3>REHABILITATION CENTER</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
                <div class="service">
                    <img src="../../assets/img/icon-15.png" alt="">
                    <h3>DENTAL IMPLANTS</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
                <div class="service">
                    <img src="../../assets/img/icon-16.png" alt="">
                    <h3>MEDICINE RESEARCH</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
                <div class="service">
                    <img src="../../assets/img/icon-11.png" alt="">
                    <h3>BLOOD BANK</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
                <div class="service">
                    <img src="../../assets/img/icon-12.png" alt="">
                    <h3>PHARMACEUTICAL ADVICE</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
                <div class="service">
                    <img src="../../assets/img/icon-13.png" alt="">
                    <h3>MEDICAL COUNSELING</h3>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nesciunt sapiente ea modi earum
                        voluptate eaque cum tenetur hic fuga </p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'ServiceSection'
}
</script>

<style lang="scss" scoped>
section {
    text-align: center;
    margin-top: 50px;
    padding-bottom: 50px;

    h1,h3{
        font-weight: 400;
    }
}

.container-sm {
    & hr {
        width: 50%;
        margin: 20px auto;
        border: 1px solid var(--color-lightgrey);
        background-color: var(--color-lightgrey);
    }
}

.offered-services {
    margin-top: 70px;
    display: flex;
    gap: 100px 30px;
    flex-wrap: wrap;
    justify-content: center;

    h3{
        margin-bottom: 15px;
    }

    & p {color:var(--color-lightdark)}
}

.service {
    max-width: calc(100% / 3 - 30px);
}
</style>