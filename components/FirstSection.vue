<template>
  <div class="parent me">
    <v-container>
      <v-row>
        <v-col cols="6" class="my-auto">
          <div class="pa-3 content">
            <h1>I'm Laurène BITOTA</h1>
            <h3>Web Developer & UI|UX Designer</h3>
            <a href="mailto:bitotalaurene@gmail.com">
              <v-btn depressed class="my-5 btn-contact" x-large>
                Contacte Me
              </v-btn>
            </a>
          </div>
        </v-col>
        <v-col cols="6">
          <img
            src="~/assets/images/me.jpg"
            alt="profile"
            width="400px"
            height="600px"
            class="profile"
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style>
.me {
  background-image: linear-gradient(rgb(254 0 123 / 0%), rgb(245 245 245 / 5%)),
    url('~/assets/images/hero.jpg') !important;
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
}
.content {
  margin-top: 110px;
}
.parent {
  background-color: #f5f5f5;
}
.btn-contact {
  background-color: #000 !important;
  border-color: #fff !important;
  color: #db2951 !important;
  font-weight: bolder;
}
.profile {
  margin-bottom: -18px;
}
</style>
