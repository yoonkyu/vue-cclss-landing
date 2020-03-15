<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar class="cc-menu-item">
        <SiteHeader v-for="link in siteHeader" :key="link.title" v-bind="link" />
      </q-toolbar>
    </q-header>
    <q-page-container>aa</q-page-container>
  </q-layout>
</template>

<script>
import SiteHeader from 'components/SiteHeader'

export default {
  name: 'MainLayout',

  components: {
    SiteHeader
  },

  data() {
    return {
      siteHeader: [
        {
          title: 'ABOUT US',
          link: '/#about-us'
        },
        {
          title: 'AD & PPL',
          link: 'https://github.com/quasarframework'
        },
        {
          title: 'RECRUIT',
          link: '/#recruit'
        }
      ]
    }
  }
}
</script>
<style scoped>
.cc-menu-item {
}
</style>
