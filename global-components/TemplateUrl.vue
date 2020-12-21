<template>
  <a target="_blank" :href="url">
    {{ text }}
    <i class="las la-external-link-square-alt"></i>
  </a>
</template>

<script>
export default {
  name: 'template-url',
  props: {
    text: {
      type: String,
      default: ''
    },
    urlTemplate: {
      type: String,
      required: true
    },
    jwt: {
      type: Boolean,
      default: true
    }
  },
  data () {
    return {
      url: ''
    }
  },
  async mounted() {
    const _ = await import('lodash')
    const moment = await import('moment')
    
    const compiler = _.template(this.urlTemplate)
    let context = { moment }
    // Add any access token
    context.jwt = this.$site.themeConfig.jwt
    this.url = compiler(context)
  }
}
</script>
