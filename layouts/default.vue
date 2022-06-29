<template>
  <div>
    <AppHeader />
    <Nuxt />
    <AppFooter />
  </div>
</template>

<script>

import AppHeader from '~/components/inc/AppHeader.vue';
import AppFooter from '~/components/inc/AppFooter.vue';
export default {
    name: 'default',
    components: {
        AppHeader,
        AppFooter
    },
    head () {
    return {
      bodyAttrs: {
        class: 'reset-body'
      }
    }
  }
}

</script>

<style lang="scss" scoped>

.reset-body {
  margin: 0px !important;
}


</style>