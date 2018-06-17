<template>
  <div v-swiper:mySwiper="swiperOption">
    <div class="swiper-wrapper">
      <div class="swiper-slide">
        <a href="https://kalisio.com">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
        <a href="https://kalisio.github.io/kaabah/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kaabah/kaabah-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
        <a href="https://kalisio.github.io/kargo/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kargo/kargo-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
        <a href="https://kalisio.gitbooks.io/krawler/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/krawler/krawler-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
         <a href="https://weacast.gitbooks.io/weacast-docs/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/weacast/weacast-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
        <a href="https://kalisio.gitbooks.io/kalisio/">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/kdk/kdk-logo-black-128x128.png" />
        </a>
      </div>
      <div class="swiper-slide">
        <a href="https:/aktnamp.com">
          <img src="https://s3.eu-central-1.amazonaws.com/kalisioscope/aktnmap/aktnmap-logo-black-128x128.png" />
        </a>
      </div>
    </div>
    <div class="swiper-pagination swiper-pagination-bullets"></div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      swiperOption: {
        autoplay: 5000,
        initialSlide: 1,
        loop: true,
        pagination: '.swiper-pagination',
        onSlideChangeEnd: swiper => {
          console.log('onSlideChangeEnd', swiper.realIndex)
        }
      }
    }
  },
  mounted() {
    import('vue-awesome-swiper')
  }
}
</script>


