<template>
  <div class="game__box" @click="onClick">
    <span>{{ value }}</span>
  </div>
</template>

<script>
export default {
  props: {
    value: String
  },
  methods: {
    onClick() {
      this.$emit("click");
    }
  }
};
</script>
