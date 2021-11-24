<template>
  <div class="rectangle">
      <Element v-for="element, index in periodicElements" :key="index" :atomicNumber="element.atomicNumber" :symbol="element.symbol"></Element>
  </div>
</template>

<script>
import * as periodicElements from '../assets/data.json'
import Element from './Element.vue'
export default {
  name: 'Table',
  components: {
    Element
  },
  data: function () {
    return {
      periodicElements: periodicElements.default
    }
  },
  methods: {
    getData () {
      console.log(periodicElements.default)
    }
  },
  mounted () {
    this.getData()
  }
}
</script>

<style>
.rectangle {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
