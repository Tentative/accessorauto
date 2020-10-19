<template>
  <v-row justify="center" class="mx-auto mt-6">
    <v-col sm="12" md="4">
      <v-img
        src="/images/home/mechanic_wipers.jpg"
        alt="Cambio tergicristalli"
        max-width="408"
        style="margin: 0 auto"
      />
    </v-col>
    <v-col sm="12" md="4">
      <v-img
        src="/images/home/mat_corner.jpg"
        alt="Vendita tappetini"
        max-width="408"
        style="margin: 0 auto"
      />
    </v-col>
    <v-col sm="12" md="4">
      <v-img
        src="/images/home/head_front_light.jpg"
        alt="Pulizia fari"
        max-width="408"
        style="margin: 0 auto"
      />
    </v-col>
  </v-row>
</template>

<style lang="scss" scoped>
@import '../assets/styles/global.scss';
@import '../layouts/global.css';

@font-face {
  font-family: 'Aero';
  src: local('Aero'), url(../assets/fonts/Aero.ttf) format('truetype');
}

html {
  font-family: 'Aero', sans-serif !important;
}

.v-application {
  font-family: 'Aero', sans-serif !important;
}
</style>
