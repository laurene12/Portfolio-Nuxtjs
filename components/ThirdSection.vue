<template>
  <div class="parent py-9">
    <v-container>
      <v-row class="intro">
        <v-col cols="12">
          <h2>Service</h2>
          <p>
            Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
            officia deserunt mollit anim id est laborum. Sed ut perspiciatis
            unde omnis iste natur
          </p>
        </v-col>
      </v-row>
      <v-row class="mb-2">
        <!--First service  -->
        <v-col cols="6">
          <v-card class="pa-8 first_service">
            <v-icon x-large class="py-5" color="white"
              >mdi-feature-search
            </v-icon>
            <h3>UX & UI Research</h3>
            <p>
              Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt
            </p>
          </v-card>
        </v-col>

        <!-- Second service -->
        <v-col cols="6">
          <v-card class="pa-8 second_service">
            <v-icon x-large class="py-5" color="white">mdi-xml </v-icon>
            <h3>Web Development</h3>
            <p>
              Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt
            </p>
          </v-card>
        </v-col>

        <!-- Third Service -->
        <v-col cols="6">
          <v-card class="pa-8 third_service">
            <v-icon x-large class="py-5" color="white">mdi-cellphone </v-icon>
            <h3>App Design</h3>
            <p>
              Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt
            </p>
          </v-card>
        </v-col>

        <!-- Four Service -->
        <v-col cols="6">
          <v-card class="pa-8 four_service">
            <v-icon x-large class="py-5" color="white">mdi-laptop </v-icon>
            <h3>Web Design</h3>
            <p>
              Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
              officia deserunt
            </p>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style>
.intro {
  text-align: center;
}
.first_service {
  color: #fff !important;
  background-image: linear-gradient(
      rgba(227, 1, 255, 99%),
      rgba(227, 1, 255, 90%)
    ),
    url('~/assets/images/service.jpg') !important;
}
.second_service {
  color: #fff !important;
  background-image: linear-gradient(
      rgba(240, 213, 0, 99%),
      rgba(240, 213, 0, 90%)
    ),
    url('~/assets/images/service.jpg') !important;
}
.third_service {
  color: #fff !important;
  background-image: linear-gradient(
      rgba(254, 58, 0, 99%),
      rgba(254, 58, 0, 90%)
    ),
    url('~/assets/images/service.jpg') !important;
}
.four_service {
  color: #fff !important;
  background-image: linear-gradient(
      rgba(254, 1, 110, 99%),
      rgba(254, 1, 110, 90%)
    ),
    url('~/assets/images/service.jpg') !important;
}
</style>
