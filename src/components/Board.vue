<template>
  <div class="game">
    <div class="game__board">
      <Square v-for="(squareValue, position) in squares" :key="position" />
    </div>
  </div>
</template>

<script>
import Square from "./Square";

export default {
  data() {
    return {
      player: "X",
      squares: Array(9).fill(null)
    };
  }
};
</script>
