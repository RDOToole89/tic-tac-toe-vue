<template>
  <div class="game">
    <div class="game__board">
      <div class="game__box" v-for="(squareValue, position) in squares" :key="position">
        <span>{{ squareValue }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      player: "X",
      squares: Array(9).fill(null)
    };
  }
};
</script>
