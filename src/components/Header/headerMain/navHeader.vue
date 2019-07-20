<template>
  <div class="navHeader">
    <div class="row">
      <div class="col-lg-6">
        <div class="navHeader__info">
          <div class="navHeader__info--title">
            <h2>Reading is the inhale, writing is the exhale.</h2>
          </div>
          <div class="navHeader__info--p">
            <p>Find the best notes of the courses from faculty like BIT, BIM, BBA and many more! And also browse out the courses, colleges, and educational events happening in Nepal</p>
          </div>
        </div>
      </div>
      <div class="col-lg-6">
        <HeaderSvg />
      </div>
    </div>
  </div>
</template>

<script>
import HeaderSvg from "./headersvg";

export default {
  components: {
    HeaderSvg
  }
};
</script>