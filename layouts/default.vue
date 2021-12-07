<template>
  <v-app>
    <v-app-bar :clipped-left="clipped" fixed app> </v-app-bar>
    <v-main class="">
      <Nuxt />
    </v-main>
    <v-footer :absolute="!fixed" app>
      <v-spacer></v-spacer>
      <span
        >Copyright &copy; {{ new Date().getFullYear() }} By Laurène BITOTA</span
      >
      <v-spacer></v-spacer>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/',
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire',
        },
      ],
    }
  },
}
</script>
<style>
.v-app-bar.v-toolbar {
  box-shadow: none !important;
}
.v-toolbar:not(.v-sheet--outlined) {
  box-shadow: none !important;
}
</style>
