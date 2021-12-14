<template>
  <section>
    <h4>WELCOME TO AVADA</h4>
    <h2>have the night of your life</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Similique
      consectetur hic delectus pariatur fugiat! Quidem, necessitatibus inventore
      corporis recusandae magni excepturi beatae soluta qui sint, amet odio.
      Enim, nulla vel?
    </p>
    <div id="halls">
      <Hall v-for="(hall, i) in halls" :key="i" :details="hall" />
    </div>
  </section>
</template>


<script>
import Hall from "@/components/Hall.vue";

export default {
  name: "Products",
  components: {
    Hall,
  },
  data() {
    return {
      halls: [
        {
          image: "../assets/img/avada-nightclub-dancelounge-small.jpg",
          url: "#",
          text: "dance lounge",
          color: "blue"
        },
        {
          image: "../assets/img/avada-nightclub-rooftoplounge-small.jpg",
          url: "#",
          text: "rooftop bar",
          color: "pink"
        },
        {
          image: "../assets/img/avada-nightclub-viplounge-small.jpg",
          url: "#",
          text: "vip lounge",
          color: "gold"
        },
        {
          image:
            "../assets/img/avada-nightclub-events-small.jpg",
          url: "#",
          text: "resident dj",
          color: "red"
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  background-image: url("../assets/img/avada-nightclub-cloud-background.jpg");
  background-size: contain;
  padding: 50px;
  h4 {
    color: #4da4dd;
    margin: 50px 0 10px 0;
  }
  h2 {
    font-size: 30px;
  }
  p{
    width: 30%;
    font-size: 15px;
    margin: 30px auto;
  }
  #halls {
    width: 42.5%;
    justify-content: center;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
  }
}
</style>