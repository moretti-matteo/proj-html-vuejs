<template>
    <section>
        <div class="container-md">
            <div class="container-sm">
                <div class="doctor-logo">
                    <img src="../../assets/img/icon-5.png" alt="doctor logo">
                </div>
                <h1>MEET OUR DOCTORS</h1>
                <hr noshade>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos perferendis cupiditate, et enim
                    asperiores rem maxime? Optio aperiam nostrum, porro eaque voluptatem explicabo nulla. Quo illo
                    explicabo consequatur maiores reiciendis.</p>
            </div>

            <div class="doctor-container">
                <div class="doctor-card">
                    <div class="doc-image">
                        <img class="image" src="../../assets/img/doctor-1.jpg" alt="">
                    </div>
                    <div class="doc-info">
                        <div>
                            <h4>JON SNOW</h4>
                            <h4>Anesthesiologist</h4>
                        </div>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <div class="doc-social">
                            <i class="fa-brands fa-facebook-square"></i>
                            <i class="fa-brands fa-twitter-square"></i>
                            <i class="fa-brands fa-instagram-square"></i>
                        </div>
                    </div>

                </div>
                <div class="doctor-card">
                    <div class="doc-image">
                        <img class="image" src="../../assets/img/doctor-2.jpg" alt="">
                    </div>
                    <div class="doc-info">
                        <div>
                            <h4>TONY STARK</h4>
                            <h4>Cardiologist</h4>
                        </div>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <div class="doc-social">
                            <i class="fa-brands fa-facebook-square"></i>
                            <i class="fa-brands fa-twitter-square"></i>
                            <i class="fa-brands fa-instagram-square"></i>
                        </div>
                    </div>

                </div>
                <div class="doctor-card">
                    <div class="doc-image">
                        <img class="image" src="../../assets/img/doctor-3.jpg" alt="">
                    </div>
                    <div class="doc-info">
                        <div>
                            <h4>ANNA SMITH</h4>
                            <h4>Nurse Practitioner</h4>
                        </div>
                        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <div class="doc-social">
                            <i class="fa-brands fa-facebook-square"></i>
                            <i class="fa-brands fa-twitter-square"></i>
                            <i class="fa-brands fa-instagram-square"></i>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'DoctorSection'
}
</script>

<style lang="scss" scoped>
section {
    margin-top: 50px;
    background-color: #f7f7f7;
    padding-bottom: 100px;
    padding-top: 50px;

}

.container-sm {
    text-align: center;

    & img {
        margin: auto;
    }

    & hr {
        width: 50%;
        margin: 20px auto;
        border: 1px solid var(--color-lightgrey);
        background-color: var(--color-lightgrey);
    }

    & h1 {
        font-weight: 400;
    }

    & p {
        color: var(--color-lightdark);
        line-height: 30px;
    }
}

.doctor-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    column-gap: 35px;
    margin-top: 50px;
}

img {
    display: block;
}

.doctor-card {
    max-width: calc(100% / 3 - 35px);
}

@media screen and(max-width:997px) {
    .doctor-card {
        max-width: calc(100% / 2 - 35px);
    }

}

@media screen and(max-width:697px) {
    .doctor-card {
        max-width: calc(100% - 35px);
    }

}

.doc-info {
    padding: 30px 30px 15px 30px;
    background-color: var(--color-white);

    &>div {
        margin-bottom: 20px;
    }

    .doc-social {
        margin-top: 40px;
        font-size: 30px;

        svg {
            margin-right: 10px;
        }
    }
}
</style>