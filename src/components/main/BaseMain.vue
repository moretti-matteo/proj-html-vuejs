<template>
    <main>
        <WelcomeSectionVue></WelcomeSectionVue>
        <DoctorSectionVue></DoctorSectionVue>
        <ServiceSectionVue></ServiceSectionVue>
    </main>
</template>

<script>
import WelcomeSectionVue from '../welcome-section/WelcomeSection.vue';
import DoctorSectionVue from '../doctor-section/DoctorSection.vue';
import ServiceSectionVue from '../services-section/ServiceSection.vue';
export default {
    name: "BaseMain",
    components: { WelcomeSectionVue, DoctorSectionVue, ServiceSectionVue }
}
</script>

<style lang="scss">
</style>