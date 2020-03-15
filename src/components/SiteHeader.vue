<template>
  <q-item clickable tag="a" target="_blank" :href="link">
    <q-item-section class="cc-vert-align">{{ title }}</q-item-section>
  </q-item>
</template>

<script>
export default {
  name: 'SiteHeader',
  props: {
    title: {
      type: String,
      required: true
    },

    link: {
      type: String,
      default: '#'
    }
  }
}
</script>
<style scoped>
.cc-vert-align {
  vertical-align: middle;
}
</style>