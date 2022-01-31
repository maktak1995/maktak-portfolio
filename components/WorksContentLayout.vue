<template>
  <div class="works-container">
    <img class="works-screenshot" :src="image" />
    <div class="works-content">
      <p class="works-explanation p-2"><slot>explanation</slot></p>
      <a v-if="url" :href="url">SITE</a>
      <a v-if="source" :href="source">SOURCE</a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: 'WorksContentLayout',
  props: {
    image: { default: '', type: String },
    url: { default: '', type: String },
    source: { default: '', type: String },
  },
}
</script>

<style>
.works-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}
.works-content {
  padding: 8px;
  padding-left: 0px;
  list-style-type: none;
  width: 100%;
}
.works-explanation {
  line-height: 28px;
}
.works-screenshot {
  width: 100%;
}
</style>
