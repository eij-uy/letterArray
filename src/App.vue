<script setup lang="ts">
import HelloWorld from "./components/HelloWorld.vue";
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
const arr: Array<any> = ["a", [1, 5]];
</script>

<template>
  <div v-for="(item, index) in arr" :key="index" class="bigNote">
    <HelloWorld :arr="item"></HelloWorld>
  </div>
</template>

<style scoped>
.bigNote {
  display: flex;
  justify-content: center;
}
</style>
