<template>
  <header>
    <navbar />
    <headerMain />
  </header>
</template>

<script>
import navbar from "./Navbar/Navbar.vue";
import headerMain from "./headerMain/navHeader.vue";
export default {
  components: {
    navbar,
    headerMain
  }
};
</script>