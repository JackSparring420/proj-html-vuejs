<template>
  <div class="hall">
    <div class="contain-img">
      <a href="details.url">
        <img :src="details.image" :alt="details.text" />
      </a>
      <div class="position-text">
        <div class="text">{{ details.text }}</div>
        <div class="color" :class="details.color"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Comic",
  props: {
    details: Object,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.hall {
  width: 50%;
  position: relative;

  .contain-img {
    width: 100%;
    height: 100%;

    img {
      object-fit: cover;
      width: 100%;
      height: 100%;
    }
  }
  .position-text {
    position: absolute;
    width: 100%;
    bottom: 15px;
    overflow: hidden;
    display: flex;
    .text {
      width: 30%;
      margin: 2px;
    }
    .color {
      width: 80%;
      height: 3px;
      position: relative;
      top: 4px;
    }
    .blue {
      background-color: #2543f1;
    }
    .pink {
      background-color: #f53c81;
    }
    .gold {
        background-color: #d5b0a1;
    }
    .red {
        background-color: #78030d;
    }
  }
}
</style>