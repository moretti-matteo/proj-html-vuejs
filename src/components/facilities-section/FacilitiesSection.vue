<template>
  <section class="section">
    
    <SectionTop></SectionTop>
    <SectionBottom></SectionBottom>
    
  </section>
</template>

<script>
import SectionBottom from './section-bottom/SectionBottom.vue';
import SectionTop from './section-top/SectionTop.vue';
export default {
    name: "FacilitiesSection",
    components: { SectionBottom, SectionTop }
};
</script>

<style lang="scss" scoped>
.section{
}
</style>