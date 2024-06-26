<script>
export default {
  name: 'DetailVue',
  props: ['title', 'brief']
}
</script>

<template>
  <article class="detail">
    <h2 class="detail-title">{{ title }}</h2>
    <p class="detail-brief">{{ brief }}</p>
  </article>
</template>

<style>
.detail {
  padding: 30px;
  text-align: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.detail-title {
  text-transform: uppercase;
}

@media screen and (min-width: 1024px) {
  .detail {
    width: 50%;
    height: 300px;
    background-color: white;
  }

  @media screen and (min-width: 1024px) {
    .detail {
      position: absolute;
      bottom: -50px;
      right: 0;
    }
  }
}
</style>
