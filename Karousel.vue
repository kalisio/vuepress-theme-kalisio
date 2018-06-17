<template>
  <carousel :autoplay="true" :autoplayHoverPause="true" :perPage="1" :paginationEnabled="true">
    <slide>
      <a href="https://kalisio.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-256x256.png" />
      </a>
    </slide>
    <slide>
       <a href="https://kalisio.github.io/kaabah/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kaabah/kaabah-logo-256x256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.github.io/kargo/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kargo/kargo-logo-256x256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/krawler/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/krawler/krawler-logo-256x256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://weacast.gitbooks.io/weacast-docs/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/weacast/weacast-logo-256x256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/kalisio/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kdk/kdk-logo-256x256.png" />
      </a>
    </slide>
    <slide>
      <a href="https:/atknamp.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/aktnmap/aktnmap-logo-256x256.png" />
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
