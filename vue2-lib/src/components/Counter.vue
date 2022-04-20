<template>
  <div>
    <h1>Counter</h1>
    <div>Button clicked: {{ counter }}</div>
    <button @click="counter++">Count</button>

    <!-- <div><canvas ref="canvas"></canvas></div> -->
    <div><canvas ref="cv"></canvas></div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue-demi';

const counter = ref(0);
// const canvas = ref<HTMLCanvasElement>();
const cv = ref<HTMLCanvasElement>();
</script>

<style>
canvas {
  border: 1px solid #000;
  margin: 5px 0;
}
</style>
