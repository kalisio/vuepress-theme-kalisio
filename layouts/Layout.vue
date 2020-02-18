<template>
  <ParentLayout>
    <Banner slot="sidebar-top"/>
  </ParentLayout>
</template>

<script>

import Banner from '@theme/components/Banner.vue'

export default {
  name: 'Layout', 
  components: {
    ParentLayout,
    Banner
  }
}
</script>
