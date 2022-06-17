<template>
    <div class="header__right">
        <nav>
            <ul>
                <li v-for="(item, i) in items" :key="i">
                    <a href="">{{ item }}</a>
                </li> 
            </ul>
        </nav>
        <button>MAKE APPOINTMENT</button>
    </div>
</template>

<script>
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
    display: flex;
    font-size: 13px;
    align-items: center;

    button {
        padding: 10px 25px;
        background-color: var(--primary-color);
        border: none;
        color: white;
        letter-spacing: 1px;
        transition: 0.25s;

        &:hover {
            cursor: pointer;
            transition: 0.25s;
            transform: scale(1.1);
        }
    }
}
</style>