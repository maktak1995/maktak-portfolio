<template>
  <div class="main">
    <Jumbotron />
    <div class="container">
      <div id="profile">
        <SectionProfile />
      </div>
      <div id="works">
        <SectionWorks />
      </div>
      <div id="contact">
        <SectionContact />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import { BootstrapVueIcons } from 'bootstrap-vue'
import 'bootstrap-vue/dist/bootstrap-vue-icons.min.css'

Vue.use(BootstrapVueIcons)

export default Vue.extend({})
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
