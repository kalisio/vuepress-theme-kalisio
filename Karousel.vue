<template>
  <carousel 
    :autoplay="true" 
    :autoplayHoverPause="true" 
    :perPage="2"
    :paginationEnabled="false">
    <slide>
      <a href="https://kalisio.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
       <a href="https://kalisio.github.io/kaabah/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kaabah/kaabah-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.github.io/kargo/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kargo/kargo-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/krawler/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/krawler/krawler-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
      <a href="https://weacast.gitbooks.io/weacast-docs/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/weacast/weacast-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/kalisio/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kdk/kdk-logo-black-128x128.png" />
      </a>
    </slide>
    <slide>
      <a href="https:/atknamp.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/aktnmap/aktnmap-logo-black-128x128.png" />
      </a>
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
