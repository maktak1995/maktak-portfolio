<template>
  <nuxt-link :to="link" class="icon-link h2"
    ><b-icon :icon="icon" /> {{ name }}</nuxt-link
  >
</template>

<script lang="ts">
export default {
  name: 'IconLink',
  props: {
    link: { default: '#home', type: String },
    icon: { default: 'house-fill', type: String },
    name: { default: 'Home', type: String },
  },
}
</script>
<style>
.icon-link {
  text-decoration: none;
  color: #212529;
  cursor: pointer;
}

.icon-link:hover {
  color: whitesmoke;
  text-decoration: none;
}
</style>
