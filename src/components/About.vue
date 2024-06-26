<script>
import Pictogram from './Pictogram.vue'
import Detail from './Detail.vue'

export default {
  name: 'CreationVue',
  components: {
    Pictogram,
    Detail
  }
}
</script>

<template>
  <div class="about">
    <Pictogram />
    <Detail
      title="The Leader In Interactive Vr"
      brief="Founded in 2011, Loopstudios has been producing world-class virtual reality projects for some of the best companies around the globe. Our award-winning creations have transformed businesses through digital experiences that bind to their brand. "
    />
  </div>
</template>

<style>
@media screen and (min-width: 1024px) {
  .about {
    position: relative;
  }
}
</style>
