<template>

  <div style="margin-top: 85px">
    <BannerTwo />
    <Feature1 />
<!--    <C2a1 />-->
    <Portfolio />
    <Testimonial />
    <Contact />
  </div>

</template>

<script>
export default {
  name: "mock",

  data() {
    return {};
  },
  components: {
    BannerTwo: () => import("@/components/shared/lp-banner/BannerTwo"),
    Feature1: () => import("@/components/custom/features/Feature1"),
    C2a1: () => import("@/components/custom/c2a/C2a1"),
    Portfolio: () => import("@/components/custom/portfolio/Portfolio"),
    Testimonial: () => import("@/components/custom/testimonial/Testimonial"),
    Contact: () => import("@/components/custom/contact/Contact"),
  },
};
</script>

<style scoped>

</style>
