<template>
  <q-page class="flex flex-center">
    <img alt="Quasar logo" src="~assets/quasar-logo-full.svg" />
  </q-page>
</template>

<script>
import VueKinesis from 'vue-kinesis'
import { Quasar, QBar } from 'quasar'
import Vue from 'vue'
export default {
  name: 'PageIndex'
}

Vue.use(Quasar, {
  components: {
    QBar
  }
})
Vue.use(VueKinesis)
</script>
