<template>
  <v-app dark>
    <Header1 />
    <v-main>
      <nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
export default {
  head() {
    return {
      title: "Harmonics Electrical | North East based Electrical Services",
      meta: [
        {
          hid: "description",
          name: "Harmonics Electrical",
          content: "High Quality Electrical Services based in North East England"
        }
      ]
    };
  },
  components: {
    Header: () => import("@/layouts/sections/Header"),
    Header1: () => import("@/components/custom/header/Header1"),
    Footer: () => import("@/layouts/sections/Footer")
  },
  methods: {}
};
</script>

<style></style>
