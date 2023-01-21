<template>
<!--  <div class="banner-wrapper" style="background-color:#439691">-->
  <v-img
    :src="require('@/assets/images/electrician-sunset.jpg')"
    class="banner-wrapper"
    max-height="800"
    gradient="to bottom, rgba(11, 28, 61, .9), rgba(0,0,0,.4)"
  >
    <v-container>
      <!-- -----------------------------------------------
            Start Banner
        ----------------------------------------------- -->
      <v-row justify="center">
        <v-col
          cols="12"
          sm="10"
          md="6"
          lg="4"
          class="d-flex align-center justify-center"
        >
          <div class="text-center">
            <h1 class="banner-title font-weight-bold white--text">
              Harmonics Electrical
            </h1>
            <h4 class="banner-subtitle mr-0 white--text font-weight-regular">
              Top Quality Electrical Services in the North-East of England
            </h4>
            <div class="mt-16 pt-2">
              <v-btn nuxt large to="#contact" color="secondary" elevation="0">
                Get In Touch
              </v-btn>
            </div>
          </div>
        </v-col>
      </v-row>

      <!-- -----------------------------------------------
            End Banner
        ----------------------------------------------- -->
    </v-container>
  </v-img>
</template>
<script>
export default {
  name: "BannerTwo",
  data() {
    return {};
  },
  methods: {}
};
</script>
