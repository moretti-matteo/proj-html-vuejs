<template>
    <div class="footer__right">
        <h3>MEDICAL DEPARTMENTS</h3>
        <hr>
        <ul>
            <li v-for="(department, i) in departments" :key="i">
                <span>
                    <i class="fa-solid fa-chevron-right"></i>
                </span>
                <a href="#">{{ department }}</a>
            </li>
        </ul>
        <button>VIEW OUR DEPARTMENTS</button>
    </div>
</template>

<script>
export default {
    name: 'MedialDepartments',
    data() {
        return {
            departments: [
                "Cardiology",
                "Pediactrics",
                "Diabetes Care",
                "Pre-natel Care",
                "Ultrasound Echocardiogram"
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.footer__right {
    a {
        color: black;
        text-decoration: none;
        margin-left: 10px;

        &:hover {
            text-decoration: underline;
            color: var(--primary-color);

        }
    }

    ul {
        list-style-type: none;

        li {
            margin-bottom: 5px;
        }
    }

    span {
        border-radius: 50%;
        background-color: var(--primary-color);
        height: 20px;
        width: 20px;
        color: white;
        font-size: 10px;
        display: inline-block;
        text-align: center;
        line-height: 20px;
    }

    hr {
        margin: 20px 0;
        width: 50px;
        background-color: var(--primary-color);
        border-color: var(--primary-color);
    }

    button {
        margin-top: 40px;
        background: var(--bg-transparent);
        padding: 10px 25px;
        transition: 0.25s;

        &:hover {
            cursor: pointer;
            color: white;
            background: var(--primary-color);
            transition: 0.25s;
            border-color: #118caa;
            transform: scale(1.1);

        }

        
    }



}
</style>