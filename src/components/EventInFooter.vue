<template>
  <div>
    <div class="separate"></div>
    <div class="event">
      <div class="contain-img">
        <img :src="details.image" :alt="details.title" />
      </div>
      <div class="text">
        <h4>{{ details.title }}</h4>
        <h5>{{ details.date }}</h5>
      </div>
    </div>
    <div class="separate"></div>
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
.event {
  display: flex;

  h4 {
    color: #4da4dd;
    margin: 10px;
  }

  .contain-img {
    width: 60px;
    height: 60px;
    margin: 5px;

    img {
      object-fit: cover;
      width: 100%;
      height: 100%;
    }
  }
  .text{
      width: 150px;
  }
}
.separate {
  height: 25px;
}
</style>