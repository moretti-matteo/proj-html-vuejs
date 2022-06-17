<template>
    <section class="hero">
        <div class="hero__content">
            <h1>
                Caring <span>For Life</span>
            </h1>
            <p>Kind words can be short and easy to speak, but their echoes are truly endless. Avada Health focuses on
                you as if it was our own family.</p>
            <button class="btn-cta">LEARN MORE</button>
        </div>
    </section>
</template>

<script>
export default {
    name: 'SectionHero'
}
</script>

<style lang="scss" scoped>
.hero {
    background-image: url('../../assets/img/header-image-homepage.jpg');
    height: 100vh;
    background-position: center;
    background-size: cover;
    position: relative;

    &__content {
        position: absolute;
        top: 40%;
        left: 40%;
        transform: translate(-40%, -40%);
        max-width: 600px;
        color: var(--color-white);

        h1 {
            font-size: 50px;
            font-weight: 300;
            margin-bottom: 20px;

            &>span {
                color: var(--primary-color);
            }
        }

        p {
            font-size: 20px;
        }

        .btn-cta {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 15px 30px;
            margin-top: 30px;
            transition: 0.25s;


            &:hover {
                cursor: pointer;
                transform: scale(1.1);
                transition: 0.25s;
                box-shadow: 0px 2px 20px 0px var(--primary-color);
            }
        }

    }
}
</style>