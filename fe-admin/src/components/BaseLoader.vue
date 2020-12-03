<template>
  <div class="base-loader">
    <vue-loaders-ball-clip-rotate-multiple scale="2" color="black"/>
  </div>
</template>

<script>
import Vue from 'vue';
import 'vue-loaders/dist/vue-loaders.css';
import VueLoaders from 'vue-loaders';
 
Vue.use(VueLoaders);
export default {
  name: 'base-loader'
}
</script>

<style>
  .base-loader {
    display: flex;
    justify-content: center;
    align-items: center;

    position: fixed;
    height: 100vh;
    width: 100vw;

    background-color: rgba(58, 55, 55, 0.267);
    z-index: 999;
  }
  .vue-loaders.ball-clip-rotate-multiple>div:first-child {
    border-right-color: #74facb !important;
    border-left-color: #74facb !important;
  }
  .vue-loaders.ball-clip-rotate-multiple>div:last-child {
    border-top-color: #4282f1 !important;
    border-bottom-color: #4282f1 !important;
  }
</style>