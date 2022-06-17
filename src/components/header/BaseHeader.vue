<template>
    <header id="head">
        <div class="container">
            <div class="header-left">
                <div class="logo">
                    <img src="../../assets/img/medical_logo_1x_light.png" alt="Logo">
                </div>
            </div>
            <div class="header-middle">
                <div>
                    <h1>Caring <span>For Life</span></h1>
                    <p>Kind words can be short and easy to speak, but their echoes are truly endless. Avada Health
                        focuses on you as if it was our own familys</p>
                    <button class="btn-cta">LEARN MORE</button>
                </div>
            </div>
            <div class="header-right">
                <ul>
                    <li v-for="(item, i) in items" :key="i">{{ item.text }}</li>
                </ul>
                <button>MAKE APPOINTMENT</button>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'BaseHeader',
    data() {
        return {
            items: [
                { text: 'HOME' },
                { text: 'ABOUT' },
                { text: 'DEPARTMENTS' },
                { text: 'ARTICLES' },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
header {
    padding-top: 20px;
    color: var(--color-white);
    height: 700px;
    background-image: url('../../assets/img/header-image-homepage.jpg');
    background-size: cover;
}

.container {
    min-height: 500px;
    display: flex;
    justify-content: space-between;
}

.header-left {
    width: 20%;
}

.logo>img {
    width: 85%;
    height: auto;
}

.btn-cta {
    padding: 10px 25px;
}

.header-middle {
    align-self: center;
    width: 40%;

    span {
        color: var(--primary-color);
    }

    &>div>* {
        margin-bottom: 20px;
    }

    & h1 {
        font-size: 40px;
        font-weight: 400;
    }
}


.header-right {
    width: 40%;
    justify-content: flex-end;


    & button {
        font-size: 13px;
    }


}

ul,
.header-right {
    display: flex;
    align-self: flex-start;
}

ul {
    list-style-type: none;
    font-size: 13px;
    margin-right: 10px;

    li {
        padding: 5px 15px;
    }
}

button {
    color: var(--color-white);
    background-color: var(--primary-color);
    border: none;
    padding: 0 15px;
    font-family: 'Zen Maru Gothic', sans-serif;
}

button:hover {
    cursor: pointer;
}
</style>