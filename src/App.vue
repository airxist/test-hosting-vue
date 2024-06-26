<template>
  <Home />
  <Main />
  <Footer />
</template>

<script>
import Home from './views/Home.vue'
import Main from './views/Main.vue'
import Footer from './views/Footer.vue'

export default {
  name: 'App',
  components: {
    Home,
    Main,
    Footer
  },
  data () {
    return {
      title: 'Loop'
    }
  }
}
</script>
