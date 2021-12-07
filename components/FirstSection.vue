<template>
  <div class="parent">
    <v-container>
      <v-row>
        <v-col cols="6" class="my-auto">
          <div class="pa-3">
            <h1>I'm Garden</h1>
            <h3>Web Developer & UI|UX Designer</h3>
            <v-btn depressed class="my-5 btn" large> Contacte Me </v-btn>
          </div>
        </v-col>
        <v-col cols="6">
          <img
            src="~/assets/images/12.png"
            alt="profile"
            width="500px"
            height="500px"
            class="profile"
          />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style>
.parent {
  background-color: #f5f5f5;
}
.btn {
  background-color: #fe0872 !important;
  border-color: #fe0872 !important;
  color: #fff !important;
}
.profile {
  margin-bottom: -18px;
}
</style>
