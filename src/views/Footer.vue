<script>
import NavMain from '../components/NavMain.vue'
import Social from '../components/Social.vue'
export default {
  name: 'FooterVue',
  components: {
    NavMain,
    Social
  },
  data () {
    return {
      navclass: 'bottom-nav'
    }
  }
}
</script>

<template>
  <footer class="footer">
    <div class="left-footer">
      <NavMain
        :navclass="navclass"
      />
    </div>
    <div class="right-footer">
      <Social />
      <small class="rights">
      {{ new Date().getFullYear() }} LoopStudios. All rights reserved</small>
    </div>
  </footer>
</template>

<style>
.footer {
  min-height: 50px;
  background-color: black;
  padding: 30px
}
.footer .logo {
  text-align: center;
}
.bottom-nav {
  list-style: none;
  text-align: center;
  margin-top: 50px;
}
.bottom-nav li {
  color: white;
  margin-top: 20px;
}
.rights {
  color: red;
  margin: 0 auto;
  display: block;
  text-align: center;
}
@media screen and (min-width: 1024px) {
  .footer {
    padding: 30px 120px;
    display: flex;
    align-items: center;
    justify-content: space-between
  }
  .footer .logo {
  text-align: unset
}
  .bottom-nav {
    display: flex;
    margin-top: 0px;
  }
  .bottom-nav li {
    margin-right: 20px
  }
  .bottom-nav li,
  .rights {
    margin-top: 10px;
  }
}
</style>
