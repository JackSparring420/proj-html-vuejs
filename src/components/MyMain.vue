<template>
    <section>
      <div id="comicslist">
        <Halls/>
        <Dj/> 
        <Events/>
      </div>
     </section>
</template>


<script>

import Halls from '@/components/Halls.vue'
import Dj from '@/components/Dj.vue'
import Events from '@/components/Events.vue'

export default {
  name: 'Products',
  components: {
    Halls,
    Dj,
    Events
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 section{
   
 }
</style>