<template>
  <Layout>
    <Banner slot="sidebar-top"/>
  </Layout>
</template>

<script>
import Layout from '@vuepress/default-theme/Layout.vue'
import Banner from '../componentes/Banner.vue'

export default {
  components: {
    Layout,
    Banner
  }
}
</script>
