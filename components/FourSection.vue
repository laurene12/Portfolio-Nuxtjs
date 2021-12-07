<template>
  <div class="main mt-8 py-5">
    <v-container>
      <v-row class="intro">
        <v-col cols="12">
          <h2>Latest Works</h2>
          <p>
            Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
            officia deserunt mollit anim id est laborum. Sed ut perspiciatis
            unde omnis iste natur
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <v-tabs color="pink accent-2" align-with-title>
            <v-tab>All</v-tab>
            <v-tab>Web Development</v-tab>
            <v-tab>App Design</v-tab>
            <v-tab>Web Design</v-tab>
            <v-tab>UI|UX Use case</v-tab>

            <v-tab-item v-for="n in 5" :key="n">
              <v-container fluid>
                <v-row>
                  <v-col v-for="i in 4" :key="i" cols="12" md="3">
                    <v-img
                      :src="`https://picsum.photos/500/300?image=${
                        i * n * 5 + 10
                      }`"
                      :lazy-src="`https://picsum.photos/10/6?image=${
                        i * n * 5 + 10
                      }`"
                      aspect-ratio="1"
                    ></v-img>
                  </v-col>
                </v-row>
              </v-container>
            </v-tab-item>
          </v-tabs>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<style>
.main {
  text-align: center;
}
</style>
