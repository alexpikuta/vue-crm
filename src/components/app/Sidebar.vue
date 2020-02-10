<template>
  <ul
    class="sidenav app-sidenav"
    :class="{open: value}"
  >
    <router-link
      v-for="link of links"
      :key="link.url"
      tag="li"
      active-class="active"
      :to="link.url"
      exact
    >
      <a
        href="#"
        class="waves-effect waves-orange pointer"
      >{{ link.title }}</a>
    </router-link>
  </ul>
</template>

<script>
export default {
  name: 'Sidebar',
  props: ['value'],
  data: () => ({
    links: [
      { title: 'Account', url: '/' },
      { title: 'History', url: '/history' },
      { title: 'Planning', url: '/planning' },
      { title: 'New Record', url: '/record' },
      { title: 'Categories', url: '/categories' },
    ],
  }),
};
</script>

<style>

</style>
