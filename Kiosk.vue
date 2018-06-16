<template>
  <carousel :autoplay="true" :autoplayHoverPause="true" :perPage="1" :navigationEnabled="true">
    <slide>
      <a href="https://kalisio.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kalisio/kalisio-logo-w256.png" />
      </a>
    </slide>
    <slide>
       <a href="https://kalisio.github.io/kaabah/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kaabah/kaabah-logo-w256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.github.io/kargo/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kargo/kargo-logo-w256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/krawler/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/krawler/krawler-logo-w256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://weacast.gitbooks.io/weacast-docs/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/weacast/weacast-logo-w256.png" />
      </a>
    </slide>
    <slide>
      <a href="https://kalisio.gitbooks.io/kalisio/">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/kdk/kdk-logo-w256" />
      </a>
    </slide>
    <slide>
      <a href="https:/atknamp.com">
        <img src="https://s3.eu-central-1.amazonaws.com/kalisio-artwork/aktnmap/aktnmap-logo-w256" />
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
