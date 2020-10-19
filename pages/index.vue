<template>
  <section id="coming-soon" style="height: 100vh; background-color: black">
    <client-only>
      <video-background
        :src="src_video"
        overlay="linear-gradient(45deg,rgba(0,0,0,.3),rgba(0,0,0.3))"
        style="max-height: 100%; height: 100vh"
      >
        <Logo />

        <ComingSoon />

        <Services />
      </video-background>
    </client-only>
  </section>
</template>

<script>
import { Logo, Services } from '~/components/'
export default {
  layout: 'work',
  components: {
    Logo,
    Services,
  },
  data() {
    return {
      message: 'Sito in costruzione',
      subtitle: 'Per info contattaci su',
      contact: 'info@accessorauto.it',
      VideoBackground: null,
      src_video: require('@/static/videos/accessorauto_intro.mp4'),
    }
  },
  mounted() {
    this.VideoBackground = require('~/plugins/vue-video-background.client.js')
  },
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/global.scss';
@import '../layouts/global.css';
@import '../assets/styles/index.scss';

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
