<template>
  <ClientOnly>
    <swiper :options="swiperOption">
      <!--swiper-slide class="kalisio"></swiper-slide>
      <swiper-slide class="kaabah"></swiper-slide>
      <swiper-slide class="kargo"></swiper-slide>
      <swiper-slide class="weacast"></swiper-slide>
      <swiper-slide class="krawler"></swiper-slide>
      <swiper-slide class="kdk"></swiper-slide>
      <swiper-slide class="aktnmap"></swiper-slide-->

      <swiper-slide>
        <a href="https://kalisio.com">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https://kalisio.github.io/kaabah/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kaabah/kaabah-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https://kalisio.github.io/kargo/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kargo/kargo-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https://kalisio.gitbooks.io/krawler/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/krawler/krawler-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https://weacast.gitbooks.io/weacast-docs/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/weacast/weacast-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https://kalisio.gitbooks.io/kalisio/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kdk/kdk-logo-black-128x128.png" />
        </a>
      </swiper-slide>
      <swiper-slide>
        <a href="https:/aktnamp.com">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/aktnmap/aktnmap-logo-black-128x128.png" />
        </a>
      </swiper-slide>
    </swiper>
  </ClientOnly>
</template>

<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'

export default {
  components: {
    Carousel,
    Slide
  },
  data() {
    return {
      swiperOption: {
        effect: 'flip',
        grabCursor: true,
        pagination: {
           el: '.swiper-pagination'
        },
        navigation: {
          nextEl: '.swiper-button-next',
          prevEl: '.swiper-button-prev'
        }
      }
    }
  }
}
</script>
