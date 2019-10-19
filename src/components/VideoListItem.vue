<template>
  <li class="list-group-item">
    <img :src="video.snippet.thumbnails.default.url" />
    {{ video.snippet.title }}
  </li>
</template>

<script>
export default {
  name: 'VideoListItem',
  props: {
    video: {
      type: Object,
      default: function() {
        return null;
      }
    }
  }
};
</script>

<style>
</style>
