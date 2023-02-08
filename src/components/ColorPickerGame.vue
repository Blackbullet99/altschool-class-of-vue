<template>
  <h1>Color Picker Game</h1>

  <div>{{ message }}</div>

  <button v-for="color in colors" :key="color" @click="matchColor(color)">
    {{ color }}
  </button>
</template>

<script>
import { useColorPickerLogic } from "../composables/color-picker-logic";

export default {
  setup() {
    return useColorPickerLogic();
  },
};
</script>

<style></style>
