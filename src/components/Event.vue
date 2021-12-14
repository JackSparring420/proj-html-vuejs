<template>
  <div class="event">
    <div class="contain-img">
      <img :src="details.image" :alt="details.title" />
    </div>
    <h4>{{ details.title }}</h4>
    <h5>{{ details.date }}</h5>
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
  width: calc(100% / 3);
  margin-bottom: 20px;
  text-align: left;

  h4 {
    color: #f53c81;
    margin: 10px;
  }

  h5 {
    margin: 10px;
  }
  .contain-img{
        border: 10px solid rgba(241, 241, 241, 0.0);
      img {
        object-fit: cover;
        object-position: 0 10px;
        width: 100%;
        height: 100%;
      }
      }
}
</style>