<script>
import Button from './Button.vue'
import creationData from '../assets/data/creation-data.json'
import Creature from './Creature.vue'

export default {
  name: 'CreationVue',
  components: {
    Button,
    Creature
  },
  data () {
    return {
      creations: creationData
    }
  }
}
</script>

<template>
  <div class="creation">
    <div class="creation-hero">
      <h2 class="creation-title">
        Our Creations
      </h2>
      <Button text="see all" small="true" />
    </div>
    <div class="creation-board">
      <Creature
        v-for="created in creations"
        :key="created.id"
        :created="created"
      />
    </div>
    <Button text="see all" />
  </div>
</template>

<style>
.creation {
  margin: 50px 0px;
}

.creation-title {
  text-transform: uppercase;
}

.creation-board {
  margin: 10px 0px;
}

@media screen and (min-width: 1024px) {
  .creation {
    margin: 100px 0px;
  }
  .creation-hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    border: solid
  }
  .creation-board {
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: var(--cut);
  }
}
</style>
