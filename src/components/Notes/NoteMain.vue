<template>
  <div class="noteMain">
    <div class="row">
      <!--For Semester Wise -->
      <div class="col-lg-4 col-md-6 noteMain__comp" v-for="(fal,index) in Faculty" :key="index">
        <div class="noteMain__header">
          <h4>{{ fal }}</h4>
        </div>
        <div class="noteMain__links">
          <ul class="row note">
            <li class="col-6 note__items" v-for="(sem,index) in Semester" :key="index">
              <a href="#" class="note__links">{{ sem }} Semester</a>
            </li>
          </ul>
        </div>
      </div>
      <!--For Year Wise -->
      <div class="col-lg-4 col-md-6 noteMain__comp">
        <div class="noteMain__header">
          <h4>BBS</h4>
        </div>
        <div class="noteMain__links">
          <ul class="row note">
            <li class="col-12 note__items" v-for="(yr,index) in Year" :key="index">
              <a href="#" class="note__links_year">{{ yr }} Year</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["Faculty"],
  data() {
    return {
      Semester: ["1st", "2nd", "3rd", "4th", "5th", "6th", "7th", "8th"],
      Year: ["1st", "2nd", "3rd", "4th"]
    };
  }
};
</script>
