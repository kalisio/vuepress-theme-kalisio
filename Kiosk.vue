<template>
  <carousel>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kalisio/kalisio-logo-256x112.png" style="width: 300px; max-width: 100%;" />
    </slide>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kaabah/kaabah-logo-256x112.png" style="width: 300px; max-width: 100%;" />
    </slide>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kargo/kargo-logo-256x112.png" style="width: 300px; max-width: 100%;" />      
    </slide>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/weacast/weacast-logo-256x112.png" style="width: 300px; max-width: 100%;" />      
    </slide>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kdk/kdk-logo-256x112.png" style="width: 300px; max-width: 100%;" />      
    </slide>
    <slide>
      <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/aktnmap/aktnmap-logo-256x112.png" style="width: 300px; max-width: 100%;" />      
    </slide>
  </carousel>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'

export default {
  components: {
    Carousel,
    Slide
  }
}
</script>
