<template>
  <v-row justify="center" align="center">
    <v-col cols="12">
      <div class="text-center mb-5">
        <v-img
          srcset="../static/images/logo/main-logo-480w.png 480w,
                  ../static/images/logo/main-logo-860w.png 860w,
                  ../static/images/logo/main-logo-1240w.png 1240w"
          sizes="(max-width: 600px) 480w,
                 (max-width: 960px) 860w,
                 (min-width: 961px) 1240w,
                 1240w"
          src="../static/images/logo/main-logo-1240w.png"
          alt="Accessorauto main logo"
          >ciao ciao ciao
        </v-img>
      </div>
    </v-col>
  </v-row>
</template>

<script>
export default {
  layout: 'work',
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/index.scss';
</style>
