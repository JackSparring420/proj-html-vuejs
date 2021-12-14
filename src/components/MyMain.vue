<template>
    <section>
      <div id="comicslist">
        <Halls/> 
      </div>
     </section>
</template>


<script>

import Halls from '@/components/Halls.vue'

export default {
  name: 'Products',
  components: {
    Halls
  },
    data() {
      return {
        
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 section{
   
 }
</style>