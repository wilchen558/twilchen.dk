<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App",
  metaInfo: {
    title: 'Welcome',
    titleTemplate: '%s | Coming soon',
    meta: [
      { name: 'description', content: 'Playground for Tobias Wilchen - Web developer based in Copenhagen' },
    ]
  }
}
</script>


<style lang="scss">
</style>
