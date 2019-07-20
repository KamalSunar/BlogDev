<template>
  <div class="row events__detail" id="accordionExample">
    <div class="col-lg-6 accordion mb-5" v-for="event in events" :key="event.id">
      <div
        class="detail__data collapsed"
        data-toggle="collapse"
        :data-target="'#'+ event.id"
        aria-expanded="false"
        id="headingOne"
        :aria-controls="event.id"
        @click="selected = event.id"
        :class="{active:selected == event.id}"
      >
        <!-- when selected gets value then active will be true so active will be added in class-->
        <div class="detail__data--icon">
          <i class="fas fa-chevron-down"></i>
        </div>
        <div class="detail__data--info">
          <h4>{{ event.date }}</h4>
        </div>
        <div class="detail__data--time">
          <span>{{ event.time }}</span>
        </div>
      </div>
      <div
        class="detail__linkdrop collapse"
        :id="event.id"
        aria-labelledby="headingOne"
        data-parent="#accordionExample"
      >
        <div class="detail__linkdrop--p">
          <p>{{ event.detail }}</p>
          <a href="#">View More</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      selected: undefined,
      events: [
        {
          id: 1,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        },
        {
          id: 2,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        },
        {
          id: 3,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        },
        {
          id: 4,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        },
        {
          id: 5,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        },
        {
          id: 6,
          date: "Sunday, 25 September 2019",
          time: "12:00 AM",
          detail:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat commodi vero asperiores repudiandae facere neque. Laborum excepturi nemo, ducimus eligendi officia blanditiis obcaecati commodi tempore possimus praesentium, earum libero? Officia?"
        }
      ]
    };
  }
};
</script>