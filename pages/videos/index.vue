<template>
  <div>
    <h1>Videos</h1>
    <div v-for="video in videos" :key="video.id">
      <nuxt-link :to="`videos/${video.id}`">{{ video.name }}</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  async asyncData(context) {
    const response = await context.$axios.get(
      "http://localhost:3000/api/videos"
    );
    console.log(response);
    debugger;
  }
};
</script>

<style></style>
