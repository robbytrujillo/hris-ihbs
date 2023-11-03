<template>
  <div>
    <NuxtLogo />
    <Tutorial />
  </div>
  
</template>

<script>
import axios from 'axios'

export default {
  name: 'IndexPage',
  async asyncData({ params }) {
    const post = await axios.get('https://api.nuxtjs.dev/posts/1')
    return { post }
  },
}
</script>
