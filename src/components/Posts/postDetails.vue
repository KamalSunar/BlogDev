<template>
  <div class="row postDetail">
    <div class="col-lg-4 mb-5" v-for="post in posts" :key="post.id">
      <div class="col-lg-12 card p-0">
        <img
          class="card-img-top img-fluid"
          :src="require(`../../assets/Images/${ post.PostImg }`)"
          :alt="post.PostTitle"
        />
        <div class="card-body">
          <div class="card-icon-text">
            <div class="date">
              <i class="far fa-calendar-alt"></i>
              <p>{{ post.PostDate }}</p>
            </div>
            <div class="person">
              <i class="fas fa-user"></i>
              <p>{{ post.PostBy }}</p>
            </div>
          </div>
          <p class="card-text">{{ post.PostTitle }}</p>
        </div>
        <hr />
        <a href="#" class="card-link">Read More</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["posts"]
};
</script>