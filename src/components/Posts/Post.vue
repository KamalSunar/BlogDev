<template>
  <div class="posts">
    <div class="posts__title">
      <div class="posts__title--sideheading">
        <h3>publication</h3>
      </div>
      <div class="posts__title--heading">
        <h2>Latest posts</h2>
      </div>
      <div class="posts__title--p">
        <p>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit.
          Itaque laboriosam molestias, delectus tempora expedita incidunt cum ut velit,
          saepe porro fugit corrupti repellat temporibus aliquam sequi esse officia odit. Sint.
        </p>
      </div>
    </div>
    <div class="posts__card">
      <postDetail v-bind:posts="Posts" />
    </div>
  </div>
</template>

<script>
import postDetail from "./postDetails.vue";

export default {
  data() {
    return {
      Posts: [
        {
          id: 1,
          PostImg: "luffy.jpg",
          PostDate: "10 feb 2018",
          PostBy: "Captain",
          PostTitle: "Old questions of 2018 BIT with solved answers."
        },
        {
          id: 2,
          PostImg: "zoro.jpg",
          PostDate: "10 feb 2018",
          PostBy: "Vice Captain",
          PostTitle: "Top 5 Colleges to start your career in IT."
        },
        {
          id: 3,
          PostImg: "sanji.jpg",
          PostDate: "10 feb 2018",
          PostBy: "Vice Captain",
          PostTitle: "Best Management college with affordable price."
        }
      ]
    };
  },
  components: {
    postDetail
  }
};
</script>
