<template>
  <main>
    <WelcomeSectionVue></WelcomeSectionVue>
    <DoctorSectionVue></DoctorSectionVue>
    <ServiceSectionVue></ServiceSectionVue>
    <FacilitiesSection></FacilitiesSection>
    <AppointmentSection></AppointmentSection>
  </main>
</template>

<script>
import WelcomeSectionVue from "../welcome-section/WelcomeSection.vue";
import DoctorSectionVue from "../doctor-section/DoctorSection.vue";
import ServiceSectionVue from "../services-section/ServiceSection.vue";
import FacilitiesSection from "../facilities-section/FacilitiesSection.vue";
import AppointmentSection from "../appointment-section/AppointmentSection.vue";
export default {
  name: "BaseMain",
  components: {
    WelcomeSectionVue,
    DoctorSectionVue,
    ServiceSectionVue,
    FacilitiesSection,
    AppointmentSection
},
};
</script>

<style lang="scss">
</style>