<script setup lang="ts">
import dayjs from 'dayjs';
import HelloWorld from './components/HelloWorld.vue'
import { Person } from '@w4ng3/tools'

const p = new Person("Junmping", "math");
</script>

<template>
  <div>
    <div>当前时间{{ dayjs().format('YYYY年MM月DD日 HH:mm:ss') }}</div>
    <div>{{ p.name }} : {{ p.slogan }}</div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
