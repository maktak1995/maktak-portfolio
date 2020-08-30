<template>
  <div class="section">
    <div class="section-header">
      <div class="h1"><b-icon :icon="icon" /> {{ title }}</div>
    </div>
    <div class="section-content">
      <slot> section-content </slot>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'SectionLayout',
  props: {
    icon: { default: 'house-fill', type: String },
    title: { default: 'Home', type: String },
  },
}
</script>

<style>
.section {
  padding-top: 148px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.section-content {
  padding-top: 24px;
  padding-bottom: 24px;
}
</style>
