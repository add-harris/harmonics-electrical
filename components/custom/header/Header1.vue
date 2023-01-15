<template>
  <div>
    <!-- -----------------------------------------------
          Start Header
    ----------------------------------------------- -->
    <v-app-bar
      app
      class="app-header navbar-light header1"
      flat
      absolute
      elevate-on-scroll
    >
      <v-container class="py-0 fill-height">
        <!-- Logo -->
        <div class="logo-small">
          <NLink to="/">
            <v-img
              :src="require('@/assets/images/harmonics-electrical-logo.png')"
              alt="logo"
            />
          </NLink>
        </div>

        <v-spacer></v-spacer>
        <v-btn class="d-block d-md-none" text @click="toggleClass()">
          <v-app-bar-nav-icon />
        </v-btn>
        <!-- Desktop view Navigation -->
        <div
          class="navigation"
          v-bind:class="[isActive ? 'd-block' : '']"
          @click="isActive = !isActive"
        >
          <ul class="navbar-nav">
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="#services"> Services </n-link>
            </li>
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="#our-work"> Our Work </n-link>
            </li>
            <li class="nav-item" text>
              <n-link class="nav-link" nuxt to="#reviews"> Reviews </n-link>
            </li>
          </ul>
        </div>
        <v-btn
          class="d-none d-lg-flex btn-custom-nm ml-5"
          nuxt
          outlined
          color="primary"
          to="#contact"
          elevation="0"
        >
          Contact Us
        </v-btn>
      </v-container>
    </v-app-bar>
    <!-- -----------------------------------------------
          End Header
    ----------------------------------------------- -->
  </div>
</template>

<script>
export default {
  name: "Header1",
  data() {
    return {
      isActive: false,
    };
  },
  methods: {
    toggleClass: function (event) {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style>

.logo-small {
  width: 130px
}

</style>
