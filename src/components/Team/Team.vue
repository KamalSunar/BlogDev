<template>
  <section class="team">
    <div class="team__sideheader">
      <h3>human beings</h3>
    </div>
    <div class="team__header">
      <h2>Our awesome team</h2>
    </div>

    <div class="row">
      <div class="col-lg-6" v-for="(person,index) in persons" :key="index">
        <a href="#" class="team__members">
          <div class="team__members--img">
            <img :src="require(`../../assets/Images/${ person.Img }`)" :alt="person.Name" />
          </div>
          <div class="team__members--detail">
            <div class="team__members--details">
              <h3 class="team__member--Name">{{ person.Name }}</h3>
              <h5 class="team__member--field">{{ person.Skill }}</h5>
            </div>
          </div>
        </a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      persons: [
        {
          Name: "Monkey D. Luffy",
          Skill: "Straw Hat Captain",
          Img: "luffy.jpg"
        },
        {
          Name: "Roronoa Zoro",
          Skill: "Straw Hat Vice Captain",
          Img: "zoro.jpg"
        },
        {
          Name: "Vinsmoke Sanji",
          Skill: "Straw Hat Cook",
          Img: "sanji.jpg"
        },
        {
          Name: "Cat burglar Nami",
          Skill: "Straw Hat Navigator",
          Img: "nami.jpg"
        },
        {
          Name: "God Ussop",
          Skill: "Straw Hat Sniper",
          Img: "ussop.jpg"
        },
        {
          Name: "Nico Robin",
          Skill: "Straw Hat Archaeologist",
          Img: "robin.jpg"
        }
      ]
    };
  }
};
</script>