<template>
  <article class="w-64 h-64 bg-white rounded m-8 border shadow-md card">
    <header class="h-16 pl-4 pt-3 pb-2">
      <h3 class="title">{{ title }}</h3>
      <p class="flex">
        <span
          class="star-active value"
          v-for="activeStar in value"
          :key="`activeStar-${activeStar}`"
          >★</span
        >
        <span
          class="star-inactive value"
          v-for="inactiveStar in 5 - value"
          :key="`inactiveStar-${inactiveStar}`"
          >★</span
        >
      </p>
    </header>
    <p class="overflow-x-auto h-48 px-4 py-2 border-t message">
      {{ message }}
    </p>
  </article>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true,
    },
    message: {
      type: String,
      required: true,
    },
    value: {
      type: Number,
      required: true,
    },
  },
};
</script>

<style>
.star-active {
  color: #ffcc33;
}

.star-inactive {
  color: #c0c0c0;
}
</style>