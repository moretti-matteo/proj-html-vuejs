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
            <button class="play" @click="toggleModal()"></button>
            <div class="modal">
                <div class="modal__close">
                    <button @click="toggleModal()">X</button>
                </div>
                <div class="modal__content"></div>
            </div>

        </div>
    </div>
</template>

<script>
import gsap from 'gsap';
export default {
    name: 'SectionTop',
    data() {
        return {
            modalActive: false,
            posY: 0
        }
    },
    methods: {
        toggleModal() {
            let tl = gsap.timeline();
            if (!this.modalActive) {
                tl.to('.modal', { scale: 1, display: 'block', duration: 1, ease: "expo.out" });
            } else {
                tl.to('.modal', { scale: 0, display: 'none', duration: 0.7, ease: "expo" });
            }
            this.modalActive = !this.modalActive;
        },
        onScroll() {
            this.posY = window.top.scrollY;
            // console.log(this.posY);

            if (this.posY > 3450 || this.posY < 2500) {
                if (this.modalActive) {
                    this.toggleModal();
                }
            }
        }
    },
    mounted() {
        window.addEventListener("scroll", this.onScroll)
    },
    beforeDestroy() {
        window.removeEventListener("scroll", this.onScroll)
    }
}
</script>

<style lang="scss" scoped>
.modal {
    position: absolute;
    left: 50%;
    top: 50%;
    height: 75%;
    width: 65%;
    border: 2px solid var(--primary-color);
    padding: 0;
    background-color: rgba(0, 0, 0, 25%);
    backdrop-filter: blur(7px);

    transform: translate(-50%, -50%) scale(0);

    // &:after{
    //     content: "";
    //     position: absolute;
    //     right:0;
    //     top:0;
    //     height: 25px;
    //     width: 25px;
    //     font-size: 20px;
    //     color:red;
    // }


    &__close {
        display: flex;
        justify-content: flex-end;

        & button {
            border: 1px solid white;
            padding: 5px 10px;
            color: var(--primary-color);
            background: rgba(0, 0, 0, 20%);

            &:hover {
                cursor: pointer;
            }
        }


    }

    &__content {
        background-image: url('https://i.ytimg.com/vi/c21QZnQtGqo/maxresdefault.jpg');
        background-size: cover;
        background-position: bottom;
        height: 90%;
        width: 90%;
        margin: 0 auto;
    }
}


.section__top {
    position: relative;
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

    .play:active {
        transform: scale(0.9);
    }
}
</style>