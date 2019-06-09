<template>
  <a-tooltip title="Tempo trabalhado">
    <a-progress :percent="30" />
  </a-tooltip>
</template>


<script>
export default {
  name: 'Progress',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
