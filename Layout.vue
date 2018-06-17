<template>
  <Layout>
    <Carousel slot="sidebar-top"/>
  </Layout>
</template>

<script>
import Layout from '@default-theme/Layout.vue'
import Carousel from './Carousel.vue'

export default {
  components: {
    Layout,
    Carousel
  }
}
</script>
