<template>
  <div>
    <b-button
      v-b-modal="`my-modal-${title}`"
      :style="{ backgroundImage: `url(${image})` }"
      class="modal-button"
    >
    </b-button>
    <b-modal :id="`my-modal-${title}`" hide-footer :title="title" size="lg"
      ><slot>modal content</slot></b-modal
    >
  </div>
</template>

<script lang="ts">
export default {
  name: 'ImageButtonModal',
  props: {
    image: { default: '', type: String },
    title: { default: '', type: String },
  },
}
</script>

<style>
.modal-button {
  background: center no-repeat;
  background-size: cover;
  background-color: rgba(255, 255, 255, 0.6);
  background-blend-mode: lighten;
  width: 240px;
  height: 240px;
}
</style>
