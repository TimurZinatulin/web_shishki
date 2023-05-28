<template>
  <div id="app">
    <component :is="layout">
      <router-view />
    </component>
  </div>
</template>

<script>
import EmptyLayout from '@/layouts/EmptyLayout'
import MainLayout from '@/layouts/MainLayout'
import ExtraLayout from '@/layouts/ExtraLayout'

export default {
  computed: {
    layout() {
      return this.$route.meta.layout + '-layout';
    }
  },
  components: {
    EmptyLayout, MainLayout, ExtraLayout
  }
}
</script>

<style>
@import 'templates/main_page.css';
</style>
