<template>
    <a-button class="btn" type="primary" :size="size" :icon="icon" >{{name}}</a-button>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
      size: 'large',
    }
  },
  props:{
    name: String,
    icon: String
  }
}
</script>

<style>

</style>
