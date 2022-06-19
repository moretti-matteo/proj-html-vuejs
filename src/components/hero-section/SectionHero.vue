<template>
    <section class="hero">
        <div class="hero__content">
            <h1 class="fade-in">
                Caring <span>For Life</span>
            </h1>
            <p class="fade-in">Kind words can be short and easy to speak, but their echoes are truly endless. Avada
                Health focuses on
                you as if it was our own family.</p>
            <button class="btn-cta cta-gsap">LEARN MORE</button>
        </div>
    </section>
</template>


<script>
import gsap from 'gsap';

export default {
    name: 'SectionHero',
    mounted() {
        let tl = gsap.timeline();
        tl.to(".fade-in", { opacity: 1, y: 0, duration: 1, stagger: 0.3 });
        tl.to(".cta-gsap", { y: 0, duration: 1.3, opacity: 1 }, "0");
    }

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

        .fade-in {
            opacity: 0;
            transform: translateY(2rem);
        }

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

        .cta-gsap {
            opacity: 0;
            transform: translateY(2rem);

        }

        .btn-cta {
            background-color: var(--primary-color);
            color: white;
            border: none;
            padding: 15px 30px;
            margin-top: 30px;



            &:hover {
                cursor: pointer;
            }
        }

    }
}
</style>