<template>
  <m3Header></m3Header>
  <marqueeCompo></marqueeCompo>
  <instantEstimateCompo></instantEstimateCompo>
  <instantValueEstimatorFormCompo></instantValueEstimatorFormCompo>
  <aboutUsCompoVue></aboutUsCompoVue>
  <footerCompVue></footerCompVue>
</template>

<script>
import m3Header from "./components/m3-header.vue";
import marqueeCompo from "./components/marquee-compo.vue";
import instantEstimateCompo from "./components/instant-estimate-compo.vue";
import instantValueEstimatorFormCompo from "./components/instant-value-estimator-form.vue";
import aboutUsCompoVue from "./components/about-us-compo.vue";
import footerCompVue from "./components/footer-comp.vue";
export default {
  name: "App",
  components: {
    m3Header,
    marqueeCompo,
    instantEstimateCompo,
    instantValueEstimatorFormCompo,
    aboutUsCompoVue,
    footerCompVue,
  },
};
</script>

<style></style>
