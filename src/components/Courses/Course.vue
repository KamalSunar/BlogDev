<template>
  <section>
    <div class="row courses">
      <div class="col-lg-6">
        <!-- course Image Section -->
        <div class="courses__img">
          <CourseImg />
        </div>
      </div>
      <div class="col-lg-6">
        <!-- course Details Section -->
        <div class="courses__details">
          <div class="courses__details--smallheader">
            <h3>Courses you should to see</h3>
          </div>
          <div class="courses__details--header">
            <h2>Carefully Choose The Course Before Your Degree</h2>
          </div>
          <p class="courses__details--main">
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
            Molestiae, delectus obcaecati autem voluptas quibusdam enim
            numquam reiciendis expedita sapiente incidunt voluptatem aliquam esse
            iure asperiores facilis quae mollitia. Culpa, rerum?
          </p>
          <a href="javascript:void(0)" class="btn">view all courses</a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import CourseImg from "./CourseImg.vue";
export default {
  components: {
    CourseImg
  }
};
</script>