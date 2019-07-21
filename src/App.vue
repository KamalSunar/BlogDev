<template>
  <div id="app">
    <Header />
    <main class="container">
      <Notes />
      <Course />
      <Events />
      <Speech />
      <Team />
      <Posts />
    </main>
    <Newsletter />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header/Header.vue";
import Notes from "./components/Notes/Notes.vue";
import Course from "./components/Courses/Course.vue";
import Events from "./components/Events/Events.vue";
import Speech from "./components/speech/Speech.vue";
import Team from "./components/Team/Team.vue";
import Posts from "./components/Posts/Post.vue";
import Newsletter from "./components/Newsletter/newsletter.vue";
import Footer from './components/Footer/Footer.vue';

export default {
  name: "app",
  components: {
    Header,
    Notes,
    Course,
    Events,
    Speech,
    Team,
    Posts,
    Newsletter,
    Footer
  }
};
</script>

<style>
@import "./assets/styles/css/style.css";
</style>
