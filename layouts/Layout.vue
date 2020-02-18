<template>
  <ParentLayout>
    <Banner slot="sidebar-top"/>
  </ParentLayout>
</template>

<script>
import ParentLayout from '@parent-theme/layouts/Layout.vue'
import Banner from '@theme/components/Banner.vue'

export default {
  name: 'Layout', 
  components: {
    ParentLayout,
    Banner
  }
}
</script>
