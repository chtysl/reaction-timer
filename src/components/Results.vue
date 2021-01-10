<template>
  <div v-if="score < 300">Super fast {{ score }}ms</div>
  <div v-else-if="score < 600">Kinda fast {{ score }}ms</div>
  <div v-else-if="score < 2500">Super slow {{ score }}ms</div>
  <div v-else>Slow as snail {{ score }}ms</div>
</template>

<script>
export default {
  props: ["score"],
};
</script>

<style >
</style>