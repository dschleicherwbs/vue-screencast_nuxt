<template>
  <div>
    <h1>We are in video {{ video.name }}</h1>
    <nuxt-link :to="`${video.id}/edit`">
      <v-btn>Edit</v-btn>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: ["video"]
};
</script>

<style>
</style>
