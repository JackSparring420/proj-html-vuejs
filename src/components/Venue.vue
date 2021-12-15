<template>
  <div>
    <div class="separate"></div>
    <div class="event">
      <div class="contain-img">
        <img :src="details.image" :alt="details.title" />
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

  h4 {
    color: #4da4dd;
    margin: 10px;
  }

  .contain-img {
    width: 250px;
    height: 100px;
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