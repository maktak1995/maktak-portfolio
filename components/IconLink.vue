<template>
  <div :href="link" class="iconLink h2"><b-icon :icon="icon" /> {{ name }}</div>
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
.iconLink {
  cursor: pointer;
}

.iconLink:hover {
  color: whitesmoke;
}
</style>
