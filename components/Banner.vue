<template>
  <p align="center">
    <a :href="link">
	    <img :src="image" />
    </a>
	  <br />
	  <i v-if="slogan">
      <small>{{slogan}}</small>
    </i>
	  <i v-if="version">
      <small>{{version}}</small>
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
      image: this.image,
      slogan: this.slogan,
      link: this.link
    }
  },
  created () {
    if (this.$site.themeConfig.banner) {
      if (this.$site.themeConfig.banner.image) this.image = this.$site.themeConfig.banner.image
      if (this.$site.themeConfig.banner.slogan) this.slogan = this.$site.themeConfig.banner.slogan
      if (this.$site.themeConfig.banner.link) this.link = this.$site.themeConfig.banner.link
    }

  }
}
</script>
