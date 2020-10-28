<template>
  <div>
    <hideButton @click="hideStar = !hideStar" />
    <div class="flex flex-wrap">
      <card
        class="card"
        v-bind:class="{ 'hide-star': hideStar }"
        v-for="review in reviews"
        :title="review.title"
        :message="review.message"
        :value="review.value"
        :key="review.id"
      />
    </div>
  </div>
</template>

<script>
import Card from "~/components/Card.vue";
import hideButton from "~/components/hide_button.vue";

export default {
  components: { Card, hideButton },
  data() {
    return {
      hideStar: false,
      reviews: [
        {
          title: "カードタイトル1",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 3,
          id: 1,
        },
        {
          title: "カードタイトル2",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 1,
          id: 2,
        },
        {
          title: "カードタイトル3",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 4,
          id: 3,
        },
        {
          title: "カードタイトル4",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 2,
          id: 4,
        },
        {
          title: "カードタイトル5",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 5,
          id: 5,
        },
        {
          title: "カードタイトル6",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 4,
          id: 6,
        },
        {
          title: "カードタイトル7",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 2,
          id: 7,
        },
        {
          title: "カードタイトル8",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 1,
          id: 8,
        },
        {
          title: "カードタイトル9",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 3,
          id: 9,
        },
        {
          title: "カードタイトル10",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 3,
          id: 10,
        },
        {
          title: "カードタイトル11",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 1,
          id: 11,
        },
        {
          title: "カードタイトル12",
          message:
            "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quod assumenda libero amet odit obcaecati sed facilis? Non voluptatem expedita molestiae asperiores repudiandae laudantium blanditiis velit harum explicabo quidem? Et, delectus?",
          value: 4,
          id: 12,
        },
      ],
    };
  },
};
</script>

<style scoped>
</style>