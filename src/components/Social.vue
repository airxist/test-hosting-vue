<script>
import twitter from '../assets/images/icon-twitter.svg'
import facebook from '../assets/images/icon-facebook.svg'
import instagram from '../assets/images/icon-instagram.svg'
import pinterest from '../assets/images/icon-pinterest.svg'
export default {
  name: 'SocialVue',
  data () {
    return {
      twitter: twitter,
      facebook: facebook,
      instagram: instagram,
      pinterest
    }
  }
}
</script>

<template>
  <div class="social">
    <li>
      <img :src="twitter" alt="twitter">
    </li>
    <li>
      <img :src="facebook" alt="twitter">
    </li>
    <li>
      <img :src="instagram" alt="twitter">
    </li>
    <li>
      <img :src="pinterest" alt="twitter">
    </li>
  </div>
</template>

<style>
.social {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
  margin: 40px auto 10px;
}
@media screen and (min-width: 1024px) {
  .social {
    margin: 0 auto;
    justify-content: end;
    gap: 10px
  }
}
</style>
