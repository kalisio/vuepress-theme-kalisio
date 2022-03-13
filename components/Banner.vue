<template>
  <p align="center">
    <a  v-if="image" :href="link">
	    <img :src="image" />
    </a>
	  <br />
	  <i v-if="slogan">
      <small>{{slogan}}</small>
    </i>
    <br />
	  <i v-if="version">
      <small>{{version}}</small>
    </i>    
  </p>
</template>

<script>
export default {
  name: 'banner',
  data () {
    return {
      image: undefined,
      slogan: undefined,
      version: undefined,
      link: '#'
    }
  },
  created () {
    if (this.$site.themeConfig.banner) {
      if (this.$site.themeConfig.banner.image) this.image = this.$site.themeConfig.banner.image
      if (this.$site.themeConfig.banner.slogan) this.slogan = this.$site.themeConfig.banner.slogan
      if (this.$site.themeConfig.banner.version) this.version = this.$site.themeConfig.banner.version
      if (this.$site.themeConfig.banner.link) this.link = this.$site.themeConfig.banner.link
    }

  }
}
</script>
