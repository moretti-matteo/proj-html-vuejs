<template>
    <main>
        <WelcomeSectionVue></WelcomeSectionVue>
        <DoctorSectionVue></DoctorSectionVue>
    </main>
</template>

<script>
import WelcomeSectionVue from '../welcome-section/WelcomeSection.vue';
import DoctorSectionVue from '../doctor-section/DoctorSection.vue';
export default {
    name: "BaseMain",
    components: { WelcomeSectionVue, DoctorSectionVue }
}
</script>

<style lang="scss">
</style>