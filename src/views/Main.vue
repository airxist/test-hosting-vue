<template>
  <main class="content">
    <About />
    <Creation />
  </main>
</template>

<script>
import About from '../components/About.vue'
import Creation from '../components/Creation.vue'

export default {
  name: 'MainVue',
  components: {
    About,
    Creation
  }
}
</script>

<style>
.content {
  min-height: 200px;
  padding: 30px;
}

@media screen and (min-width: 1024px) {
  .content {
    padding: 30px 120px;
  }
}
</style>
