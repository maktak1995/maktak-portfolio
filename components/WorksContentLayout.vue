<template>
  <div class="works-container">
    <img class="works-screenshot" :src="image" />
    <ul class="works-content">
      <li>
        <div class="works-li">
          <div class="pr-2">URL:</div>
          <a v-if="url" :href="url">{{ url }}</a>
          <p v-else>非公開</p>
        </div>
      </li>
      <li>
        <div class="works-li">
          <div class="pr-2">Source:</div>
          <a v-if="source" :href="source">{{ source }}</a>
          <p v-else>非公開</p>
        </div>
      </li>
      <p class="works-explanation p-2"><slot>explanation</slot></p>
    </ul>
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
.works-li {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  border-bottom: 1px solid #66d7ff;
  padding: 5px;
  margin: 2px;

  & p {
    margin-bottom: 0px;
  }
}
.works-explanation {
  line-height: 28px;
}
.works-screenshot {
  width: 320px;
}
</style>
