<template>
    <nav>
      <ul>
        <li v-for="(link, i) in navLeft" :key="i">
          <a :href="link.url" :class="link.active ? 'active' : ''">{{ link.text }}</a>
        </li>
      </ul>
        <img src="../assets/img/avada-nightclub-logo-2x-200x66.png" alt="" />
      <ul>
        <li v-for="(link, k) in navRight" :key="k">
          <a :href="link.url" :class="link.active ? 'active' : ''">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
</template>

<script>
export default {
  name: "Header",
  props: {
    navLeft: Array,
    navRight: Array,
  },

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
nav {
  width: 70%;
  padding: 50px;
  display: flex;
  justify-content: space-between;
  margin: auto;
  ul {
    font-size: 13px;
    position: relative;
    top: 6px;
    width: 33%;
    display: flex;
    list-style-type: none;
    justify-content: space-between;
    align-items: center;
    a {
        color: white;
        text-decoration: none;
    }
  }
  .active {
    color: #be80a4;
    border-bottom: 2px solid #be80a4;
    padding: 3px;
  }
}
</style>
