<template>
  <article class="w-64 h-64 bg-white rounded m-8 border shadow-md">
    <header class="h-16 pl-4 pt-3 pb-2">
      <h3 class="">{{ reviews[0].title }}</h3>
      <aside>
        <!-- <span id="cssTest" v-for="n in 5" :key="n">★</span> -->
        <span id="cssTest" v-for="n in limitCount" :key="n">★</span>
      </aside>
    </header>
    <p class="overflow-x-auto h-48 px-4 py-2 border-t">
      {{ reviews[0].message }}
    </p>
  </article>
</template>

<script>
export default {
  data() {
    return {
      reviews: [
        {
          title: "カードタイトル1",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 3,
        },
        {
          title: "カードタイトル2",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 1,
        },
        {
          title: "カードタイトル3",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 4,
        },
      ],
    };
  },
  computed: {
    limitCount() {
      return this.reviews[0].value;
    },
  },
};
</script>

<style>
#cssTest {
  color: #ffcc33;
}
</style>