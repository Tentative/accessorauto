<template>
  <v-row justify="center" align="center" class="mx-auto">
    <v-col cols="12">
      <v-img
        srcset="/images/logo/main-logo-480w.png 480w,
                  /images/logo/main-logo-860w.png 860w"
        sizes="(max-width: 600px) 480px,
                 (max-width: 960px) 960px,
                 960px"
        src="/images/logo/main-logo-960w.png"
        alt="Accessorauto main logo"
        class="mt-5"
        max-width="960px"
        style="margin: 0 auto"
      >
      </v-img>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'Logo',
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/global.scss';
@import '../layouts/global.css';
</style>
