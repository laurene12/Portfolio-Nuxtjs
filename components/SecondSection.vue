<template>
  <div>
    <v-container>
      <v-row class="py-8">
        <v-col cols="5">
          <div>
            <h2>About Me</h2>
          </div>
        </v-col>
        <v-col cols="7">
          <div>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
              eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut
              enim ad minim veniam, quis nostrud exercitation ullamco laboris
              nisi ut aliquip ex ea commodo consequat.
            </p>
            <p>
              Duis aute irure dolor in reprehenderit in voluptate velit esse
              cillum dolore eu fugiat nu pariatur excepteur sint occaecat.
            </p>
          </div>
          <div>
            <v-btn depressed class="my-5 mr-3 btn" large> View Works </v-btn>
            <v-btn depressed outlined class="my-5 btn-outlined" large>
              Download CV
            </v-btn>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style>
.btn {
  background-color: #fe0872 !important;
  border-color: #fe0872 !important;
  color: #fff !important;
}

.btn-outlined {
  background-color: transparent !important;
  border-color: #fe0872 !important;
  color: #fe0872 !important;
}
</style>
