<template>
  <div  class="home">
    <Nav />
    <h1 class="hero-title">
      IMMERSIVE EXPERIENCES THAT DELIVER
    </h1>
  </div>
</template>

<script>
import Nav from '../components/Nav.vue'

export default {
  name: 'HomeVue',
  components: {
    Nav
  }
}
</script>

<style>
.home {
  min-height: 100vh;
  background-image: url(../assets/images/mobile/image-hero.jpg);
  padding: 20px 30px;
}

.hero-title {
  margin-top: 30vh;
  color: white;
  width: 100%;
  border: solid 2px white;
  padding: 10px
}

@media screen and (min-width: 1024px) {
  .home {
    background-image: url(../assets/images/desktop/image-hero.jpg);
    padding: 50px 120px;
  }

  .hero-title {
    width: 50vw;
  }
}
</style>
