<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div class="target" v-motion-slide-visible-once-left>
  </div>
  <div class="target" v-motion-slide-visible-once-bottom></div>
  <div
    class="target"
    v-motion
    :initial="{
      opacity: 0,
      y: 100,
    }"
    :enter="{
      opacity: 1,
      y: 0,
    }"
  />
  
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  
}
body{
  background-color: #000;
  margin: 0;
}
.target{
  width: 300px;
  height: 300px;
  margin: 300px auto 500px auto;
  background-color: aquamarine;

}
</style>
