<template>
  <p align="center">
    <a :href="linkUrl">
	    <img :src="imageSource" />
    </a>
	  <br />
	  <i v-if="sloganContent">
      <small>{{sloganContent}}</small>
    </i>
  </p>
</template>

<script>
export default {
  name: 'banner',
  props: {
    image: {
      type: String,
      default: 'https://s3.eu-central-1.amazonaws.com/kalisioscope/kalisio/kalisio-logo-black-256x84.png'
    },
    title: {
      type: String,
      default: 'Unleashing the potential of spatial information'
    },
    link: {
      type: String,
      default: 'https://kalisio.com'
    }
  },
  data () {
    return {
      imageSource: this.image,
      sloganContent: this.slogan,
      linkUrl: this.link
    }
  },
  created () {
    if (this.$site.themeConfig.banner) {
      if (this.$site.themeConfig.banner.image) this.imageSource = this.$site.themeConfig.banner.image
      if (this.$site.themeConfig.banner.slogan) this.sloganContent = this.$site.themeConfig.banner.slogan
      if (this.$site.themeConfig.banner.link) this.linkUrl = this.$site.themeConfig.banner.link
    }

  }
}
</script>
