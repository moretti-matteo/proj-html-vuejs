<template>
    <div class="header__right">
        <nav>
            <ul>
                <li v-for="(item, i) in items" :key="i">
                    <a href="">{{ item }}</a>
                </li>
            </ul>
        </nav>
        <a href="#appointment">MAKE APPOINTMENT</a>
    </div>
</template>

<script>
import gsap from 'gsap';
export default {
    name: 'HeaderRight',
    data() {
        return {
            items: [
                "HOME",
                "ABOUT",
                "DEPARTMENTS",
                "ARTICLES",
            ]
        };
    },
    mounted() {
        let tl = gsap.timeline();
        tl.to(".header__right", { y: 0, opacity: 1, duration: 1.3, ease: "power4.out" });
    }
}
</script>

<style lang="scss" scoped>
.header__right ul li {
    display: inline-block;
    margin-right: 25px;

    &:first-child a {
        color: var(--primary-color);
    }

    a {
        text-decoration: none;
        color: white;

        &:hover {
            color: var(--primary-color);
        }
    }

}

.header__right {
    transform: translateY(-100px);
    opacity: 0;
    display: flex;
    font-size: 13px;
    align-items: center;

    &>a {
        transition: 0.25s;
        letter-spacing: 1px;
        color: white;
        text-decoration: none;
        padding: 10px 25px;
        background-color: var(--primary-color);


        &:hover {
            cursor: pointer;
            transition: 0.25s;
            transform: scale(1.1);
        }
    }
}
</style>