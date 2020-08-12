<template lang="html">
  <div id="app">
    <div class="news">
      <h1>Latest SpaceX Mission</h1>
      <h2>{{ news.name }}</h2>
      <img :src="news.links.patch.small":width = "400" :height = "400">
      <p>{{ news.details }}</p>
      <br>
    </div>
  </div>

</template>

<script>

export default {
  name: 'news-feed',
  props: ['news']
}
</script>

<style lang="css" scoped>

/* .news {
  text-align: left;
  width: 96%;
  border-style: solid;
  padding: 10px
} */
</style>
