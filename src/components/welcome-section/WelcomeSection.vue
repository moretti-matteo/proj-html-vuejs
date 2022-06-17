<template>
    <section>
        <div class="container-md">
            <div class="container-sm">
                <h1>Welcome to Avata Health</h1>
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Vel optio quas placeat minima, sit
                    consequuntur cum quibusdam accusantium totam?</p>
            </div>

            <div class="card-section">
                <div>
                    <div class="img-container">
                        <img class="image" src="../../assets/img/icon-1.png" alt="">
                    </div>
                    <h3>SAME DAY APPOINTMENTS</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
                <div>
                    <div class="img-container">
                        <img class="image" src="../../assets/img/icon-2.png" alt="">
                    </div>
                    <h3>WORLD CLASS FACILITIES</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
                <div>
                    <div class="img-container">
                        <img class="image" src="../../assets/img/icon-3.png" alt="">
                    </div>
                    <h3>EXPERT DOCTORS</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>
                <div>
                    <div class="img-container">
                        <img class="image" src="../../assets/img/icon-4.png" alt="">
                    </div>
                    <h3>COMPLEMENTARY TERAPHY</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
                </div>

            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'WelecomeSection',
}
</script>

<style lang="scss" scoped>
section {
    margin-top: 50px;
    text-align: center;
}

.container-sm {
    &>h1 {
        font-weight: 400;
        margin-bottom: 20px;
    }

    p {
        line-height: 35px;
    }
}

.image {
    width: 25%;
}



.card-section {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-top: 60px;
    color: var(--color-lightdark);

    &>div {
        max-width: 25%;
    }
    & h3 {
        font-weight: 400;
    }

    &>div>* {
        margin-bottom: 20px;
    }
}
</style>