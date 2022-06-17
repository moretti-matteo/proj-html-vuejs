<template>
    <div class="section__bottom">
        <div class="card">
            <div>
                <h4>Emergency Care</h4>
            </div>
            <div>
                <img src="../../../assets/img/wave-divider.png" alt="" />
            </div>
            <div>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
                    nostrum ipsa excepturi perfere
                </p>
            </div>
            <div>
                <button>LEARN MORE</button>
            </div>
        </div>
        <div class="card">
            <div>
                <h4>Expert Diagnostics</h4>
            </div>
            <div>
                <img src="../../../assets/img/wave-divider.png" alt="" />
            </div>
            <div>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
                    nostrum ipsa excepturi perfere
                </p>
            </div>
            <div>
                <button>LEARN MORE</button>
            </div>
        </div>
        <div class="card">
            <div>
                <h4>Superb Rehabilitation</h4>
            </div>
            <div>
                <img src="../../../assets/img/wave-divider.png" alt="" />
            </div>
            <div>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. At,
                    nostrum ipsa excepturi perfere
                </p>
            </div>
            <div>
                <button>LEARN MORE</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "SectionBottom"
}
</script>

<style lang="scss" scoped>
.section__bottom {
    display: flex;
    text-align: center;
    color: var(--color-white);

    $colors: #3aafbf #3597c3 #327ec7;

    @for $i from 1 through 3 {
        &>div:nth-child(3n + #{$i}) {
            background-color: nth($colors, $i);
        }
    }

    &>div {
        padding: 40px 15px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: calc(100% / 3);

        button {
            background: none;
            border: 1px solid white;
            color: white;
            padding: 10px 25px;
            transition: 0.25s;
            margin-top: 10px;

            &:hover {
                cursor: pointer;
                transform: scale(1.1);
                background: rgba(0, 0, 0, 25%);
                color: white;
                transition: 0.25s;
            }
        }

        &>* {
            margin-bottom: 5px;
        }
    }
}
</style>