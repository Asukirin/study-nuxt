<template>
  <article class="w-64 h-64 bg-white rounded m-8 border shadow-md">
    <header class="h-16 pl-4 pt-3 pb-2">
      <h3 class="">{{ review_title }}</h3>
      <aside class="">
        <span>★</span>
        <span>★</span>
      </aside>
    </header>
    <p class="overflow-x-auto h-48 px-4 py-2 border-t">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda
      libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae
      asperiores repudiandae laudantium blanditiis velit harum explicabo quidem?
      Et, delectus?
    </p>
  </article>
</template>

<script>
export default {
  data() {
    return {
      // items: [{ review_title: "カードタイトル" }],
      review_title: "カードタイトル",
    };
  },
};
</script>

<style>
</style>