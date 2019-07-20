<template>
  <section>
    <div class="notes">
      <div class="notes__heading">
        <h2>Browse the Notes</h2>
      </div>
      <div class="notes__links">
        <NoteMain v-bind:Faculty="Faculty" />
      </div>
    </div>
  </section>
</template>

<script>
import NoteMain from "./NoteMain.vue";
export default {
  data() {
    return {
      Faculty: ["bit", "bba", "bim", "bsw", "bhm", "bttm", "bca", "bba-m"]
    };
  },
  components: {
    NoteMain
  }
};
</script>