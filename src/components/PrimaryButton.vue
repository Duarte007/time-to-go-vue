<template>
  <div id="button">
    <a-button type="primary" block>{{name}}</a-button>
  </div>
</template>

<script>

export default {
  name: 'app',
  props:{
    name: String,
  }
}
</script>

<style>


</style>
