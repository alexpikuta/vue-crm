<template>
  <div class="app-main-layout">
    <Navbar @open-sidebar="navIsOpen = !navIsOpen" />
    <Sidebar v-model="navIsOpen" />

    <main
      class="app-content"
      :class="{full: !navIsOpen}"
    >
      <router-view />
    </main>

    <div class="fixed-action-btn">
      <a
        class="btn-floating btn-large blue"
        href="#"
      >
        <i class="large material-icons">add</i>
      </a>
    </div>
  </div>
</template>
<script>
import Navbar from '@/components/app/Navbar.vue';
import Sidebar from '@/components/app/Sidebar.vue';

export default {
  name: 'MainLayout',
  components: {
    Navbar,
    Sidebar,
  },
  data: () => ({
    navIsOpen: true,
  }),
};
</script>
