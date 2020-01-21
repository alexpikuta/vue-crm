<template>
  <div id="app">
    <component :is="layout" />
  </div>
</template>

<script>
import AuthLayout from '@/layouts/AuthLayout.vue';
import MainLayout from '@/layouts/MainLayout.vue';

export default {
  components: {
    AuthLayout,
    MainLayout,
  },
  computed: {
    layout() {
      return `${this.$route.meta.layout || 'auth'}-layout`;
    },
  },
};
</script>

<style lang="sass">
  @import '~materialize-css/dist/css/materialize.min.css'
  @import 'assets/styles.css'
</style>
