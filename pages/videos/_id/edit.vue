<template>
  <div>
    <h1>Editing {{ video.name }}</h1>
    <nuxt-link :to="`/videos/${video.id}`">
      <v-btn>back</v-btn>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: ["video"]
};
</script>

<style lang="scss" scoped>
</style>