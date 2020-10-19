<template>
  <section id="coming-soon">
    <no-ssr>
      <video-background
        :src="src_video"
        style="height: 100vh"
        overlay="linear-gradient(45deg,rgba(0,0,0,.3),rgba(0,0,0.3))"
      >
        <Logo />

        <ComingSoon />

        <Services />
      </video-background>
    </no-ssr>
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
