<template>
    <section>
      <div id="comicslist">
        <Halls/>
        <Dj/> 
        <Events/>
        <VipLonge/>
      </div>
     </section>
</template>


<script>

import Halls from '@/components/Halls.vue'
import Dj from '@/components/Dj.vue'
import Events from '@/components/Events.vue'
import VipLonge from '@/components/VipLonge.vue'

export default {
  name: 'Products',
  components: {
    Halls,
    Dj,
    Events,
    VipLonge
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
 section{
   
 }
</style>