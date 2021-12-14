<template>
    <section>
        <div id="contain">
          <h4>SPECIAL EVENT</h4>
          <h2>for your diary</h2>
        <div id="events">
            <Event v-for="event, i in events" :key="i" :details="event"/> 
        </div>
        <button>RSVP NOW</button>
        </div>
     </section>
</template>


<script>

import Event from '@/components/Event.vue'

export default {
  name: 'Events',
  components: {
    Event
  },
    data() {
      return {
          events: [
  {
    image: "../assets/img/avada-nightclub-events-1.jpg",
    title: "DJ Fusion",
    date: "August 19, 2021 @ 8:00am",
  },
  {
    image: "../assets/img/avada-nightclub-events-2.jpg",
    title: "House Nation",
    date: "August 19, 2021 @ 8:00am",
  },
  {
    image: "../assets/img/avada-nightclub-events-3.jpg",
    title: "Jazz Night",
    date: "August 19, 2021 @ 8:00am",
  },
  {
    image: "../assets/img/avada-nightclub-events-4.jpg",
    title: "VIP Taster Sessions",
    date: "August 19, 2021 @ 8:00am",
  },
  {
    image: "../assets/img/avada-nightclub-events-5.jpg",
    title: "Fanky House Rave",
    date: "August 19, 2021 @ 8:00am",
  },
  {
    image: "../assets/img/avada-nightclub-events-6.jpg",
    title: "Urban Vibes",
    date: "August 19, 2021 @ 8:00am",
  }
]
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 section{
   background-image: url("../assets/img/avada-nightclub-homepage-events-background-new.jpg");
   background-size: cover;

    #contain {
        padding: 100px 0;
        background-color: rgba(0, 0, 0, 0.507);
        h4 {
            color: #f53c81;
        }
    
        h2{
            font-size: 35px;
        }
    
         #events {
            width: 70%;
            margin: auto;
            display: flex;
            flex-wrap: wrap;
          }
    
          button {
                background-color: #f53c81;
                color: white;
                border: 1px solid #f53c81;
                padding: 10px 20px;
          }
    }

 }
</style>