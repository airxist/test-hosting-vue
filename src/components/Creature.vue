<script>
export default {
  name: 'CreatureVue',
  props: ['created']
}
</script>

<template>
  <div class="creature">
    <h3 class="creature-title">{{ created.title }}</h3>
  </div>
</template>

<style>
.creature {
  width: 100%;
  height: 150px;
  border: solid 2px blue;
  margin-top: 20px;
}
@media screen and (min-width: 1024px) {
  .creature {
    width: calc((100% / 4) - var(--cut));
    height: 400px;
  }
}
</style>
