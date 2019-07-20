<template>
  <section class="events">
    <div class="events__title">
      <div class="events__title--sideheading">
        <h3>useful information</h3>
      </div>
      <div class="events__title--heading">
        <h2>Upcoming Events</h2>
      </div>
      <div class="events__title--p">
        <p>
          Lorem ipsum dolor sit amet consectetur, adipisicing elit.
          Mollitia, facilis? Illo tempore distinctio possimus, quia,
          nemo nam natus numquam temporibus error exercitationem suscipit
          fuga in maiores asperiores nesciunt, culpa sed.
        </p>
      </div>
    </div>
    <div class="events__details">
        <EventDetail />
    </div>
  </section>
</template>

<script>
import EventDetail from "./eventDetails.vue";

export default {
  components: {
      EventDetail
  }
};
</script>