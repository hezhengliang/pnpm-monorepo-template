<!--
 * @Date: 2022-11-26 14:35:49
 * @LastEditors: 93eryi@gmail.com
 * @LastEditTime: 2023-06-18 11:48:56
 * @Description: 
-->


<template>
  <div>
    Turbo Cache Test =>{{ turboCacheUpdate}}
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
    <Text />
  </div>
</template>
<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
// import TestVue from './components/TestVue.vue'
import { ref} from 'vue'
import { isFunction} from '@mp/shared'
import { Text } from '@mp/components'
function a(){
  console.log('a is Function');
  
}
const turboCacheUpdate = ref(true)
console.log(isFunction(a), turboCacheUpdate);

</script>
<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
