<template>
  <article class="w-64 h-64 bg-white rounded m-8 border shadow-md">
    <header class="h-16 pl-4 pt-3 pb-2">
      <h3>{{ title }}</h3>
      <p class="flex star">
        <span
          class="star-active"
          v-for="activeStar in value"
          :key="`activeStar-${activeStar}`"
          >★</span
        >
        <span
          class="star-inactive"
          v-for="inactiveStar in 5 - value"
          :key="`inactiveStar-${inactiveStar}`"
          >★</span
        >
      </p>
    </header>
    <p class="overflow-x-auto h-48 px-4 py-2 border-t scroll-none">
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

<style scoped>
.star-active {
  color: #ffcc33;
}

.star-inactive {
  color: #c0c0c0;
}

.hide-star .star {
  display: none;
}

.scroll-none {
  -ms-overflow-style: none;
  scrollbar-width: none;
}

.scroll-none::-webkit-scrollbar {
  display: none;
}
</style>