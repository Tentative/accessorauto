<template>
  <section>
    <v-row justify="center" align="center" class="mx-auto mt-6">
      <div
        class="text-center text-uppercase text-lg-h5 text-sm-h5"
        style="color: #a91c17"
      >
        {{ message }}
      </div>
    </v-row>
    <v-row justify="center" align="center" class="mx-auto">
      <div
        class="text-center text-uppercase text-lg-h5 text-sm-h5"
        style="color: #a91c17"
      >
        <span>{{ subtitle + ' ' }}</span
        ><span style="color: white !important"
          ><a href="mailto:info@accessorauto.it">{{ contact }}</a></span
        >
      </div>
    </v-row>
  </section>
</template>

<script>
export default {
  name: 'ComingSoon',
  data() {
    return {
      message: 'Sito in costruzione',
      subtitle: 'Per info contattaci su',
      contact: 'info@accessorauto.it',
    }
  },
}
</script>

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
