<template>
  <div>
    <div>My blog navigation bar here</div>
    <Nuxt />
  </div>
</template>

<script>
export default {
  layout: 'blog',
  // OR
  layout(context) {
    return 'blog'
  },
  middleware: ['auth'],
}
</script>
