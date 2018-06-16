<template>
  <Layout>
    <Kiosk slot="sidebar-top"/>
  </Layout>
</template>

<script>
import Layout from '@default-theme/Layout.vue'
import Kiosk from './Kiosk.vue'

export default {
  components: {
    Layout,
    Kiosk
  }
}
</script>
