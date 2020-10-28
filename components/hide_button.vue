<template>
  <button
    @click="handleClick"
    class="border border-black rounded-full py-2 px-4"
  >
    評価表示切替
  </button>
</template>

<script>
export default {
  methods: {
    handleClick(e) {
      this.$emit("click", e);
    },
  },
};
</script>

<style scoped>
</style>