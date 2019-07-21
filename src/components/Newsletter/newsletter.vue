<template>
  <section class="jumbotron newsletter">
    <div class="container">
      <div class="row">
        <div class="col-lg-5 newsletter__text">
          <h4>Subscribe to our newsletter</h4>
        </div>
        <div class="col-lg-7 newsletter__input">
          <form>
            <input
              type="email"
              v-model="email"
              class="newsletter__input--box"
              placeholder="freebies@sales.com"
            />
            <button class="submit_btn" type="submit">Subscribe</button>
          </form>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      email: ""
    };
  }
};
</script>