<template>
  <main>
    <WelcomeSectionVue></WelcomeSectionVue>
    <DoctorSectionVue></DoctorSectionVue>
    <ServiceSectionVue></ServiceSectionVue>
    <FacilitiesSection></FacilitiesSection>
    <AppointmentSection></AppointmentSection>
    <CarouselSection></CarouselSection>
  </main>
</template>

<script>
import WelcomeSectionVue from "../welcome-section/WelcomeSection.vue";
import DoctorSectionVue from "../doctor-section/DoctorSection.vue";
import ServiceSectionVue from "../services-section/ServiceSection.vue";
import FacilitiesSection from "../facilities-section/FacilitiesSection.vue";
import AppointmentSection from "../appointment-section/AppointmentSection.vue";
import CarouselSection from "../carousel-section/CarouselSection.vue"

export default {
  name: "BaseMain",
  components: {
    WelcomeSectionVue,
    DoctorSectionVue,
    ServiceSectionVue,
    FacilitiesSection,
    AppointmentSection,
    CarouselSection
},
};
</script>

<style lang="scss">
</style>