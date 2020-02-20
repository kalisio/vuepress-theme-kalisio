

<template>
  <iframe 
    id="kano" 
    title="Kano" 
    allow="geolocation *" 
    allowfullscreen style="width: 100%; height: 60vh" 
    frameBorder="0"
    src="https://kano.test.kalisio.xyz">
  </iframe>
</template>

<script>
import postRobot from 'post-robot'

export default {
  name: 'kano',
  mounted() {
    this.kano = document.getElementById('kano').contentWindow
    this.component = 'map'
    postRobot.on('kano-ready', () => {
      postRobot.send(kano, 'setLocalStorage', {
        'kano-jwt': 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJhdWQiOiJkZXYua2FsaXNpby54eXoiLCJpc3MiOiJrYWxpc2lvIiwiZXhwIjoxNTg0MDE1Mjg0fQ.oOPo_7lPMFgH6dBUtSnNs3w4h-DwwCSLdg9yMF0YU18'
      }).then(_ => postRobot.send(this.kano, this.component))
    })
  }
};
</script>
