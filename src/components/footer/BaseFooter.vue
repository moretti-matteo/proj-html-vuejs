<template>
    <footer>
        <div class="footer__top container">
            <DescAgency></DescAgency>
            <ContactInformation></ContactInformation>
            <MedicalDepartments></MedicalDepartments>
        </div>
        <div class="footer__bottom">
            <div class="container">
                <FooterCopyright></FooterCopyright>
            </div>
        </div>
    </footer>
</template>

<script>
import ContactInformation from '../contact-information/ContactInformation.vue';
import MedicalDepartments from '../medical-departments/MedicalDepartments.vue';
import DescAgency from '../desc-agency/DescAgency.vue';
import FooterCopyright from '../copyright/FooterCopyright.vue'
export default {
    name: "BaseFooter",
    components: { ContactInformation, MedicalDepartments, DescAgency, FooterCopyright }
}
</script>

<style lang="scss">
footer {

    .footer__top.container {
        margin-top: 50px;
        padding-bottom: 50px;
        display: flex;
        gap: 20px;
        justify-content: space-between;
        flex-wrap: wrap;

        & h3 {
            font-weight: 400;
        }

        &>div {
            width: calc(100% / 3 - 20px);
        }

    }


    .footer__bottom {
        padding: 20px 0;
        background-color: #eee;
    }
}
</style>