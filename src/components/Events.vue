<template>
    <section>
      <div id="events">
        <Comic v-for="event, i in events" :key="i" :details="event"/> 
      </div>
      <button id="load">RSVP NOW</button>
     </section>
</template>


<script>

import Comic from '@/components/Comic.vue'

export default {
  name: 'Events',
  components: {
    Comic
  },
    data() {
      return {
          events: [
  {
    image: "../assets/img/avada-nightclub-events-1.jpg",
    title: "DJ Fusion",
    date: "Action Comics",
  },
  {
    image: "../assets/img/avada-nightclub-events-2.jpg",
    title: "House Nation",
    date: "Action Comics",
  },
  {
    image: "../assets/img/avada-nightclub-events-3.jpg",
    title: "Jazz Night",
    date: "Action Comics",
  },
  {
    image: "../assets/img/avada-nightclub-events-4.jpg",
    title: "VIP Taster Sessions",
    date: "Action Comics",
  },
  {
    image: "../assets/img/avada-nightclub-events-5.jpg",
    title: "Fanky House Rave",
    date: "Action Comics",
  },
  {
    image: "../assets/img/avada-nightclub-events-6.jpg",
    title: "Urban Vibes",
    date: "Action Comics",
  }
]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 section{
     background-color: black;
     padding: 50px 0;
     #events {
        width: 70%;
        margin: auto;
        display: flex;
        flex-wrap: wrap;
      }

      #load {
            background-color: #f53c81;
            color: white;
            border: 1px solid #f53c81;
            padding: 10px 20px;
      }
 }
</style>