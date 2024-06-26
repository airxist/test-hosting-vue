<script>
import logo from '../assets/images/logo.svg'
export default {
  name: 'NavMainVue',
  props: ['navclass'],
  data () {
    return {
      logo: logo
    }
  }
}
</script>

<template>
  <div class="logo">
    <img :src="logo" alt="logo" />
  </div>
  <nav :class="navclass">
    <li>About</li>
    <li>Careers</li>
    <li>Events</li>
    <li>Products</li>
    <li>Support</li>
  </nav>
</template>
