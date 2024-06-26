<script>
import figure from '../assets/images/desktop/image-interactive.jpg'

export default {
  name: 'PictogramVue',
  data () {
    return {
      picture: figure
    }
  }
}
</script>

<template>
  <div class="pictogram">
    <img :src="picture" alt="pictVue" />
  </div>
</template>

<style>
.pictogram {
  width: 100%
}

.pictogram img {
  width: 100%;
  height: 100%
}

@media screen and (min-width: 1024px) {
  .pictogram {
    width: 60%;
    height: 450px;
  }
}
</style>
