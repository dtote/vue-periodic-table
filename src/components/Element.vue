<template>
<div class="square">
  <div>{{atomicNumber}}</div>
  <div>{{symbol}}</div>
</div>
</template>

<script>
export default {
  name: 'Element',
  props: ['atomicNumber', 'symbol']
}
</script>

<style scoped>
.square{
    border: 1px solid black;
    height: 100px;
    width: 100px;
    background-color: pink;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
</style>
