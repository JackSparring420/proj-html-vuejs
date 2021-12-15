<template>
  <section>
    <div class="contain">
      <div id="events">
        <h3>EVENTS</h3>
        <EventInFooter v-for="(event, i) in events" :key="i" :details="event" />
      </div>
      <div id="contact">
        <img
          class="underline margin"
          src="../assets/img/avada-nightclub-logo-2x-200x66.png"
          alt=""
        />
        <ul>
          <li
            v-for="(contact, k) in contacts"
            :key="k"
            :class="contact.active ? 'active' : ''"
          >
            {{ contact.text }}
          </li>
        </ul>
        <div class="icons">
          <i class="fab fa-facebook-f"></i>
          <i class="fab fa-twitter"></i>
          <i class="fab fa-instagram"></i>
          <i class="fab fa-youtube"></i>
        </div>
      </div>
      <div id="venues">
        <h3>VENUES</h3>
        <Venue v-for="(venue, i) in venues" :key="i" :details="venue" />
      </div>
    </div>
      <div id="registred">
          &copy; copyright 2012 - 2021 | Avada Theme by <a href="#">ThemeFusion</a> | All rights Reserved | Powered by <a href="#">WordPress</a>
      </div>
  </section>
</template>


<script>
import EventInFooter from "@/components/EventInFooter.vue";
import Venue from "@/components/Venue.vue";
export default {
  name: "MyFooter",
  components: {
    EventInFooter,
    Venue,
  },
  data() {
    return {
      events: [
        {
          image: "../assets/img/avada-nightclub-events-1.jpg",
          title: "DJ Fusion",
          date: "August 19, 2021 @ 8:00 am",
        },
        {
          image: "../assets/img/avada-nightclub-events-2.jpg",
          title: "House Nation",
          date: "August 19, 2021 @ 8:00 am",
        },
        {
          image: "../assets/img/avada-nightclub-events-3.jpg",
          title: "Jazz Night",
          date: "August 19, 2021 @ 8:00 am",
        },
      ],
      venues: [
        {
          image: "../assets/img/avada-nightclub-footer-rooftop.jpg",
          title: "DJ Fusion",
        },
        {
          image: "../assets/img/avada-nightclub-footer-dancelounge.jpg",
          title: "House Nation",
        },
      ],
      contacts: [
        {
          text: "Avada NightClub",
          active: false,
        },
        {
          text: "100 Night Club Blvd",
          active: false,
        },
        {
          text: "Beverly Hills",
          active: false,
        },
        {
          text: "hi@your-domain.com",
          active: true,
        },
        {
          text: "+1 (555) 000 000",
          active: false,
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section {
  background-image: url("../assets/img/avada-nightclub-footer-background-final-2.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: bottom;
  padding: 100px;

  .contain {
    display: flex;
    justify-content: space-between;
    width: 70%;
    margin: auto;

    h3 {
      margin-top: 28px;
    }

    ul {
      list-style-type: none;
    }
    .active {
      color: #4da4dd;
    }

    ul {
      margin-top: 35px;
      li {
        margin: 5px;
      }
    }

    .icons {
      margin-top: 35px;
      i {
        margin: 15px;
      }
    }
  }

  #registred {
      margin-top: 100px;
      a {
          color: #4da4dd;
      }
  }
}
</style>