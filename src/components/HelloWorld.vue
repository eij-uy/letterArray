<script lang="ts" setup>
const props = defineProps({
  arr: String || Array<any>,
});
</script>

<template>
  <div class="miniNote" v-for="(item, index) in arr" :key="index">
    {{ item }}
  </div>
</template>

<style scoped>
.miniNote {
  width: 30px;
  height: 30px;
}
</style>
