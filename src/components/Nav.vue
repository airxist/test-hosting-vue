<template>
  <div class="nav-bar">
    <NavMain
      :navclass="navclass"
    />
    <span class="nav-toggle" @click="toggleNav('show')">
      <img :src="toggler" alt="toggler" />
    </span>
  </div>
</template>

<script>
import toggler from '../assets/images/icon-hamburger.svg'
import NavMain from './NavMain.vue'
export default {
  name: 'NavVue',
  components: {
    NavMain
  },
  data () {
    return {
      toggler: toggler,
      navclass: 'nav-main'
    }
  },
  methods: {
    toggleNav (type) {
      this.navclass = `nav-main ${type}`
    }
  }
}
</script>

<style>
.nav-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.nav-main {
  position: absolute;
  background-color: black;
  width: 100%;
  height: 100vh;
  top: 0;
  left: -100%;
  transition: .2s;
  padding-left: 30px;
  list-style: none;
}

.nav-main.show {
  left: 0
}

.nav-main li {
  color: white;
  cursor: pointer;
}

.nav-toggle {
  display: block;
}

@media screen and (min-width: 1024px) {
  .nav-bar {}
  .nav-main {
    position: static;
    width: fit-content;
    height: unset;
    background-color: transparent;
    display: flex;
    align-items: center;
    gap: 30px;
  }
  .nav-toggle {
    display: none;
  }
}
</style>
