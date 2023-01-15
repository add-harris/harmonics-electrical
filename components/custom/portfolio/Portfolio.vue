<template>
  <div>
    <div class="portfolio-component mini-spacer" id="our-work">
      <v-container>
        <!-- -----------------------------------------------
            Start Portfolio Text
        ----------------------------------------------- -->
        <v-row justify="center">
          <v-col cols="12" sm="10" md="9" lg="7">
            <div class="text-center">
              <h2 class="section-title font-weight-medium">
                Our Recent work with three column
              </h2>
              <p>
                You can relay on our amazing features list and also our customer
                services will be great experience for you without doubt and in
                no-time
              </p>
            </div>
          </v-col>
        </v-row>

        <!-- -----------------------------------------------
            End Portfolio Text
        ----------------------------------------------- -->
        <!-- -----------------------------------------------
            Start Portfolio
        ----------------------------------------------- -->
        <v-row class="mt-13">
          <v-col cols="12" md="6" lg="4" v-for="example in examples" :key="example.image">
            <v-card class="portfolio-card overflow-hidden">
              <div class="portfolio-img">
                <img
                  :src=example.image
                  alt="portfolio"
                  class="img-fluid"
                />
              </div>
              <v-card-text>
                <h5 class="font-weight-medium font-18">{{example.header}}</h5>
                <p class="font-14 mb-0">{{example.text}}</p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <!-- -----------------------------------------------
            End Portfolio
        ----------------------------------------------- -->
      </v-container>
    </div>
  </div>
</template>
<script>
export default {
  name: "Portfolio",
  data() {
    return {
      examples: [
        {
          image: require("@/assets/images/bathroom.jpg"),
          header: "Title",
          text: "Some description.",
          key: "bathroom"
        },
        {
          image: require("@/assets/images/kitchen.jpg"),
          header: "Title",
          text: "Some description.",
          key: "kitchen"
        },
        {
          image: require("@/assets/images/circuitbox-outside.jpg"),
          header: "Title",
          text: "Some description.",
          key: "circuit-box"
        }
      ]
    };
  },
  methods: {},
};
</script>
