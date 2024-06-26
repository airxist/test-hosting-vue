<script>
export default {
  name: 'ButtonVue',
  props: ['text', 'small']
}
</script>

<template>
  <button :class="small ? 'btn' : 'btn large'">{{ text }}</button>
</template>

<style>
.btn {
  border: 1px black solid;
  background-color: transparent;
  padding: 10px 24px;
  display: none;
}

.btn:hover {
  background-color: black;
  color: white;
}

.btn.large {
  width: 50%;
  margin: 30px auto;
  display: block;
}

@media screen and (min-width: 1024px) {
  .btn {
    display: block
  }
  .btn.large {
    display: none
  }
}
</style>
