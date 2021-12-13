<template>
  <header>
    <NavbarHeader :navLeft="navLeft" :navRight="navRight"/>
    <div class="contain-square">
        <div class="square">
            <i class="fas fa-layer-group"></i>
            <div>Demos</div>
        </div>
        <div class="square">
            <div class="contain-price">
                <span class="value">$</span>
                <span class="price">39</span>
            </div>
            <div>
                On Sale
            </div>
        </div>
    </div>
    <div id="jumbotron">
      <img
        class="underline margin"
        src="../assets/img/avada-nightclub-homepage-image-800x398.png"
        alt=""
      />
      <h2 class="margin">making memoriesss all night long</h2>
      <div class="margin">
        <button>BECOME A VIP</button>
      </div>
      <div class="padding">
        <img
          src="../assets/img/avada-nightclub-play-showreel-200x47.png"
          alt=""
        />
      </div>
    </div>
  </header>
</template>



<script>
import NavbarHeader from "@/components/NavbarHeader.vue";

export default {
  name: "HelloWorld",
  components: {
    NavbarHeader,
  },
  data() {
    return {
      navLeft: [
        {
          text: "HOME",
          url: "#",
          here: true,
        },
        {
          text: "NIGHT",
          url: "#",
          here: false,
        },
        {
          text: "EVENTI",
          url: "#",
          here: false,
        },
      ],
      navRight: [
        {
          text: "JOBS",
          url: "#",
          here: false,
        },
        {
          text: "EVENTS",
          url: "#",
          here: false,
        },
        {
          text: "CONTACS US",
          url: "#",
          here: false,
        },
      ],
    };
  },
  //   props: {
  // msg: String
  //   },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header {
  background-image: url("../assets/img/avada-nightclub-home-hero.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  .contain-square{
      float: right;
      margin-right: 10px;
      .square{
          padding: 10px;
          background: white;
          right: 20px;
          margin: 5px;
          border-radius: 10px;
          color: gray;
          font-size: 10px;
          i{
              font-size: 20px;
              margin-bottom: 3px;
          }
          .contain-price{
              color: rgb(6, 167, 0);
              .price{
                  font-size: 20px;
              }
              .value{
                  position: relative;
                  bottom: 10px;
              }

          }
      }
  }
  #jumbotron {
    margin-top: 50px;
    .margin {
      margin-bottom: 25px;
    }
    .underline {
      border-bottom: 2px solid #4da4dd;
    }
  }
  button {
    padding: 10px;
    color: white;
    background-color: #f53c81;
    border: 1px solid #f53c81;
  }
  .padding {
    padding: 30px;
  }
}
</style>
